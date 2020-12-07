<template>
  <div class="sign_up">
      <!--START OF MAIN--->
      <main role="main">
        <div class="SignUp_container">
          <h1>Sign Up With Us!</h1>
        <p>Please fill in this form to recieve promotional offers, discounts, notices on special events, and so much more!</p>
          <div>
            <!---START OF THE SIGN UP FORM USING VEEVALIDATE-->
            <validation-observer ref="observer" v-slot="{ handleSubmit }">
              <b-form  @submit.stop.prevent="handleSubmit(submitForm)">
                <!---START OF FIRST NAME INPUT FIELD--->
                <validation-provider
                  name="first name"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
                  <b-form-group id="fname-input-group-1" label="First Name" label-for="fname-input-1">
                    <b-form-input
                      id="fname"
                      name="first name"
                      v-model="form.fname"
                      :state="getValidationState(validationContext)"
                      aria-describedby="first name-1-live-feedback"
                      placeholder="Enter First Name"
                    ></b-form-input>
                    <b-form-invalid-feedback id="first_name-1-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
                <!---END OF FIRST NAME INPUT FIELD--->
            
            <!---START OF LAST NAME INPUT FIELD--->
            <validation-provider
                  name="last name"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
                  <b-form-group id="lname-input-group-2" label="Last Name" label-for="lname-input-2">
                    <b-form-input
                      id="lname"
                      name="last name"
                      v-model="form.lname"
                      :state="getValidationState(validationContext)"
                      aria-describedby="last nanme-2-live-feedback"
                      placeholder="Enter Last Name "
                    ></b-form-input>
                    <b-form-invalid-feedback id="lname-2-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
                <!---END OF LAST NAME INPUT FIELD--->
            
            <!---START OF EMAIL INPUT FIELD--->
            <validation-provider
                  name="email address"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
                  <b-form-group id="mailaddr-input-group-3" label="Email Address" label-for="mailaddr-input-3">
                    <b-form-input
                      id="mailaddr"
                      name="mailaddr"
                      v-model="form.mailaddr"
                      :state="getValidationState(validationContext)"
                      aria-describedby="Email Address-3-live-feedback"
                      placeholder="Enter Email Address"
                    ></b-form-input>
                    <b-form-invalid-feedback id="Email Address-3-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
                <!---END OF EMAIL INPUT FIELD--->

                <!---Vue-recaptcha code including site key provided by reCAPTCHA API--->
                <div style="margin-left: 30px">
                  <vue-recaptcha sitekey="6LftB-EZAAAAAMF09-TDRdB0QhkKDUM4vFmbFtnG" 
                  @verify="enableSubmit" style="padding-top: 10px; padding-bottom: 10px;"></vue-recaptcha>
                </div>

                <!----THE GREEN SIGN UP BUTTON---->
                 <b-button type="submit" variant="success">Sign Up</b-button>
              
                <!----THE RED CANCEL BUTTON, routes back to Home page on click---->
               <router-link to="/"> <b-button class="ml-2">Cancel</b-button> </router-link> 
              </b-form>
            </validation-observer>
            <!----END OF VEEVALIDATE---->
          </div>
      </div>
    </main>
  </div>
</template>


<script>
import VueRecaptcha from 'vue-recaptcha';

export default {
  data() {
    return {
      showModal: false,
      form: {
        fname: null,
		    lname: null,
        mailaddr: null
        
      }
    };
  },
  methods: {
    getValidationState({ dirty, validated, valid = null }) {
      return dirty || validated ? valid : null;
    },

    // Resets form
    resetForm() {
      this.form = {
        fname: null,
		    lname: null,
        mailaddr: null
        
      };

      this.$nextTick(() => {
        this.$refs.observer.reset();
      });
    },
  
    // Can only be called upon validation of form via VeeValidate
    // Requires completion of reCAPTCHA to call sendEmail function
    submitForm (){
      if (this.form.disabled == false){
       this.sendEmail();
      }
    },

    // function called upon verification of reCAPTCHA, 
    enableSubmit(){
       console.log("Verified, submit button enabled");
        this.form.disabled = false;
    },
        sendEmail() {
        var fnameValue = document.getElementById("fname").value;
        var lnameValue = document.getElementById("lname").value;
        var emailValue = document.getElementById("mailaddr").value;
        var bodyValue = "<h1>Welcome, ";
        bodyValue += fnameValue;
        bodyValue += ".</h1><p>Thank you for signing up! <br>";
        bodyValue += "You will receive alerts for the latest promotional offers, special discounts and events, and more!</p>"

        //Email.send function provided by smtp.js
        // Can use either SecureToken, or plain text email credentials.
        // Plain text option is shown below but commented out
        Email.send({
          SecureToken : "7c6b77cb-8ce0-4c1b-bd02-5d37dae8493b",
          // Host : "smtp.gmail.com",
          // Username : 'cit384.final@gmail.com',
          // Password : '',
          To : emailValue,
          From : "cit384.final@gmail.com",
          Subject : "Promo Confirmation from Mexicanology",
          Body : bodyValue
          }).then((message) => {
          console.log('Message status: ', message);
          if (message == 'OK'){
            this.doNotification();}
          })
          this.resetForm();
          // Resets reCAPTCHA
          grecaptcha.reset();
    },
    // Toast notification function, this is triggered in promise of Email.send function
    doNotification() {
        this.$toast.success("Thank you for subscribing. Check your email!", {
          position: "bottom-right",
          timeout: 5000,
          closeOnClick: true,
          pauseOnFocusLoss: true,
          pauseOnHover: true,
          draggable: true,
          draggablePercent: 0.6,
          showCloseButtonOnHover: false,
          hideProgressBar: true,
          closeButton: "button",
          icon: true,
          rtl: false
        });
        // Redirects user back to Home page
        this.$router.push({ path: '/' });
    }
     
  },
  components: {
    'vue-recaptcha': VueRecaptcha
  },
}
</script>