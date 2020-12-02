<template>
  <main role="main">
  <div class="dinner">
    <!---<h1>This is an dinner page</h1>---->
    <div>
    <b-card no-body>
     <b-tabs pills card horizontal id="pills-card-tab">
      <b-tab title="Dinner" active>
          <b-card-text> *All dinner dishes are served with rice, 
              beans, and tortillas--choice of corn or flour.
          </b-card-text>
  <!------------row 1: lunch ------------------------>
    <section role="region">  
      <div class="mt-3">
      <b-card-group deck>
        <!----Shrimp Fajitas----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dinner/Skillet-Shrimp-Fajitas-Photo.jpg"
          img-alt="Shrimp Fajitas"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Shrimp Fajitas</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$17.75</b-card-sub-title>
          <b-card-text>Shrimp with grilled green and red bell peppers and onions. 
            Served with lettuce, guacamole, pico de gallo, and sour cream on the side. </b-card-text>
        </b-card-body>
        </b-card>

      <!--------Torta-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dinner/torta.jpg"
          img-alt="Torta"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Torta</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$11.75</b-card-sub-title>
           <b-card-text>A fluffy bun spread with butter and topped with refried beans, creamy avocado, cheese. It is piled on with a meat your choosing. 
             Choices: carne asada, pork, chicken, ham, pastor, or carnitas.
               </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Tostadas de ceviche-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dinner/tosdada-de-ceviche.jpg"
          img-alt="Tostadas de ceviche"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Tostadas De Ceviche</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.00</b-card-sub-title>
          <b-card-text>Fresh fish marinated in lime juice with onions, cilantro, and tomatoes. 
            Served on a crispy corn tortilla with guacamole, lettuce and sliced avocado on top.</b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
        </section>
      
  <!------------row 2: lunch ------------------------>
    <section role="region">
       <div class="mt-3">
      <b-card-group deck>
        <!----Huarache----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dinner/huaraches-700x525.jpg"
          img-alt="Huarache"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Huarache</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$15.50</b-card-sub-title>
          <b-card-text>A thick homemade corn tortilla topped with grilled chicken 
            or steak, black beans, cheese, lettuce, sour cream, pico de gallo and
             salsa verde. </b-card-text>
        </b-card-body>
        </b-card>

      <!--------Chile Relleno Burrito -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dinner/chile-relleno-burrito.jpg"
          img-alt="Chile Relleno Burrito"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chile Relleno Burrito </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.50</b-card-sub-title>
          <b-card-text>Our famous chile relleno, black beans and monterey jack cheese 
            wrapped in a large flour tortilla and topped with chipotle sauce.
          </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Taquitos Dorados-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dinner/taquitos-dorados.jpg"
          img-alt="Taquitos Dorados"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Taquitos Dorados</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.25</b-card-sub-title>
          <b-card-text>Crispy chicken or beef taquitos. Served with lettuce, cheese, 
            sour cream, gucamole, and pico de gallo.</b-card-text>
            
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
      </section>
        </b-tab>
        </b-tabs>
    </b-card>
  </div>
  <!------------END OF LUNCH TAB------------------------------------------------>
  </div>
  </main>
</template>