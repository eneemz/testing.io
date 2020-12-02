<template>
  <div id="app">
   
    <!---all pages (.vue) will have navigation bar and footer------->
    <!----MUST WRAP IT AROUND <ROUTER LINK> tag in order for 
      it to redirect you to a different 'page'-->
      <div class="navbar-menu" id="nav" role="navigation">
      <b-navbar toggleable="lg" type="dark" variant="dark">
       <b-navbar-brand href="#">Mexicanology</b-navbar-brand>
        <router-link to="/"><b-navbar-brand href="/">Home</b-navbar-brand></router-link>
        <b-dropdown text="Menu" size="lg" variant="danger">
        <router-link to="/Menu/appetizers"><b-dropdown-item href="/Menu/Appetizers.vue" title="Appetizers">Appetizers</b-dropdown-item></router-link>
        <router-link to="/Menu/breakfast"><b-dropdown-item href="/Menu/Breakfast.vue" title="Breakfast">Breakfast</b-dropdown-item></router-link>
        <router-link to="/Menu/lunch"><b-dropdown-item href="/Menu/Lunch.vue" title="Lunch">Lunch</b-dropdown-item></router-link>
        <router-link to="/Menu/dinner"><b-dropdown-item href="/Menu/Dinner.vue" title="Dinner">Dinner</b-dropdown-item></router-link>
        <router-link to="/Menu/dessert"><b-dropdown-item href="/Menu/Dessert.vue" title="Dessert">Dessert</b-dropdown-item></router-link>
        <router-link to="/Menu/drinks"><b-dropdown-item href="/Menu/Drinks.vue" title="Drinks">Drinks</b-dropdown-item></router-link>
        </b-dropdown>
        <router-link to="/contact_us"><b-navbar-brand href="/Contact_Us.vue" title="Contact Us">Contact Us</b-navbar-brand></router-link>
        <router-link to="/sign_up"><b-navbar-brand href="/Sign_Up.vue" title="Sign Up">Sign Up</b-navbar-brand></router-link>
        </b-navbar>
        </div>
    <!------END OF NAVIGATION with the use of router-link tags ----------->
     <!---- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/contact_us">Contact Us</router-link> |
      <router-link to="/sign_up">Sign Up</router-link> |
      <router-link to="/Menu/appetizers">Appetizers</router-link> |
      <router-link to="/Menu/breakfast">Breakfast</router-link> |
      <router-link to="/Menu/lunch">Lunch</router-link> |
      <router-link to="/Menu/dinner">Dinner</router-link> |
      <router-link to="/Menu/dessert">Dessert</router-link> |
      <router-link to="/Menu/drinks">Drinks</router-link>---->
    <!----END OF THE <div id="nav">--------->
    <router-view/>

    <!---START OF FOOTER-->
    <div class="footer" role="contentinfo">
        <p>
        All trademarks and registered trademarks are the property of their
        respective owners.
        </p>
        <p>© 2020 Mexicanology</p>
    </div>
    <!---END OF FOOTER-->
  </div>
  <!--END OF THE <div id="app">------>
</template>

<style>
#app {
  font-family:  Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#boot-nav{
  font-size: 15px;
  color: white;
  height: 150px;
  width: 100%;
  
  
}
#nav {
   font-family: "Times New Roman", "Amatic SC", sans-serif;
  font-size: 25px;
}
/*
#nav a {
  font-weight: bold;*/
  /*color: #2c3e50;*/
/*}*/

/*#nav*/
#app a.router-link-exact-active {
  color: #42b983;
}
</style>
