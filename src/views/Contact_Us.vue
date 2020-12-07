<template>
  <div class="contact_us">
    <!--START OF MAIN--->
      <main role="main">
        <div class="Contact_container">
          <h1>Contact Us!</h1>
          <p>Please fill in this form to send your feedback!</p>
          <div>
            <!---START OF THE CONTACT US FORM USING VEEVALIDATE-->
            <validation-observer ref="observer" v-slot="{ handleSubmit }">
              <b-form  @submit.stop.prevent="handleSubmit(submitForm)">
                <!---START OF FULL NAME INPUT FIELD--->
                <validation-provider
                  name="fullname"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
                  <b-form-group id="fullname-input-group-1" label="Full Name" label-for="fullname-input-1">
                    <b-form-input
                      id="fullname"
                      name="fullname"
                      v-model="form.fullname"
                      :state="getValidationState(validationContext)"
                      aria-describedby="fullname-1-live-feedback"
                      placeholder="Enter Full Name"
                    ></b-form-input>
                    <b-form-invalid-feedback id="fullname-1-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
            <!---END OF FULL NAME INPUT FIELD--->

            <!---START OF EMAIL ADDRESS INPUT FIELD--->
            <validation-provider
                  name="mailaddr"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
                  <b-form-group id="mailaddr-input-group-2" label="Email Address" label-for="mailaddr-input-2">
                    <b-form-input
                      id="mailaddr"
                      name="mailaddr"
                      v-model="form.mailaddr"
                      :state="getValidationState(validationContext)"
                      aria-describedby="mailaddr-2-live-feedback"
                      placeholder="Enter Email Address"
                    ></b-form-input>
                    <b-form-invalid-feedback id="mailaddr-2-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
            <!---END OF EMAIL ADDRESS INPUT FIELD--->
            
            <!---START OF SUBJECT  INPUT FIELD--->
            <validation-provider
                  name="subject"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
                  <b-form-group id="subject-input-group-3" label="Subject" label-for="subject-input-3">
                    <b-form-input
                      id="subject"
                      name="subject"
                      v-model="form.subject"
                      :state="getValidationState(validationContext)"
                      aria-describedby="subject-3-live-feedback"
                      placeholder="Subject"
                    ></b-form-input>
                    <b-form-invalid-feedback id="subject-3-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
            <!---END OF SUBJECT  INPUT FIELD--->

            <!---START OF MESSAGE  INPUT FIELD--->
            <validation-provider
                  name="message"
                  :rules="{ required: true, min: 3 }"
                  v-slot="validationContext"
                >
            <b-form-group id="message-input-group-4" label="Message" label-for="message-input-4">
                    <textarea
                      id="message"
                      name="message"
                      v-model="form.message"
                      :state="getValidationState(validationContext)"
                      aria-describedby="message-4-live-feedback"
                      cols="5"
                      rows="5"
                      placeholder="Enter your message here..."
                  ></textarea>
                  
                    <b-form-invalid-feedback id="message-4-live-feedback">{{ validationContext.errors[0] }}</b-form-invalid-feedback>
                  </b-form-group>
                </validation-provider>
                <!---END OF MESSAGE  INPUT FIELD--->
                
                <!---Vue-recaptcha code including site key provided by reCAPTCHA API--->
                <div style="margin-left: 30px">
                  <vue-recaptcha sitekey="6LftB-EZAAAAAMF09-TDRdB0QhkKDUM4vFmbFtnG" 
                  @verify="enableSubmit" style="padding-top: 10px; padding-bottom: 10px;"></vue-recaptcha>
                </div>

                <!----THE GREEN SUBMIT UP BUTTON---->
                 <b-button type="submit" variant="success">Send Message</b-button>
              
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
        fullname: null,
        mailaddr: null,
        subject: null,
        message: null,
        disabled: true
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
        fullname: null,
        mailaddr: null,
        subject: null,  
        message: null
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
      var nameValue = document.getElementById("fullname").value;
      var emailValue = document.getElementById("mailaddr").value;
      var subjectValue = document.getElementById("subject").value;
      var messageValue = document.getElementById("message").value;
      var bodyValue = "<b>New message from: </b>";
      bodyValue += nameValue;
      bodyValue += "<br>";
      bodyValue += "<b>Reply to: </b>"
      bodyValue += emailValue;
      bodyValue += "<br><br>";
      bodyValue += messageValue;

      //Email.send function provided by smtp.js
      // Can use either SecureToken, or plain text email credentials.
      // Plain text option is shown below but commented out
      Email.send({
        SecureToken : "7c6b77cb-8ce0-4c1b-bd02-5d37dae8493b",
        // Host : "smtp.gmail.com",
        // Username : "cit384.final@gmail.com",
        // Password : "",
        To : "cit384.final@gmail.com",
        From : "cit384.final@gmail.com",
        Subject : subjectValue,
        Body : bodyValue
        }).then((message) => {
        console.log('Message status: ', message);
        if (message == 'OK'){
          this.doNotification();}
        })
        // Resets form
        this.resetForm();
        // Resets reCAPTCHA
        grecaptcha.reset();
      },

      // Toast notification function, this is triggered in promise of Email.send function
      doNotification() {
        this.$toast.success("Your message has been sent!", {
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