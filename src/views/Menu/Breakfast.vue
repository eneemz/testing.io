<template>
  <main role="main">
  <div class="breakfast">
    <!-----<h1>This is an about page</h1>----->
    <div>
    <b-card no-body>
     <b-tabs pills card horizontal id="pills-card-tab">
      <b-tab title="Breakfast" active>
          <b-card-text> *All breakfast dishes are served with rice, 
              beans, and tortillas--choice of corn or flour.
          </b-card-text>

      <section role="region">
      <div class="mt-3">
      <b-card-group deck>
        <!----Huevos rancheros----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Breakfast/Huevos-rancheros.jpg"
          img-alt="Huevos rancheros"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Huevos rancheros</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$14.25</b-card-sub-title>
          <b-card-text>Consists of fried eggs served on lightly fried or charred corn or flour tortillas 
              topped with a salsa fresca made of tomatoes, chili peppers, onion, and cilantro.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Chilaquiles -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Breakfast/chilaquiles.jpg"
          img-alt="Chilaquiles"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chilaquiles </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.00</b-card-sub-title>
           <b-card-text>Corn tortillas cut in quarters and lightly fried or baked for a lighter version. 
               Green or red salsa is poured over the crisp tortilla triangles. The mixture is simmered 
               until the tortilla starts softening. Crema, crumbled queso fresco, and raw onion 
               rings, are added to the mix. 
               </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Machaca and Eggs Plate -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Breakfast/machaca and eggs.jpg"
          img-alt="Machaca and Eggs Plate"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Machaca and Eggs Plate</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.00</b-card-sub-title>
          <b-card-text>Shredded beef or chicken, green peppers, onions,
              mixed in scramble eggs.</b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
      </section>
      
  <!------------row 2: breakfast ------------------------>
      <section role="region">
       <div class="mt-3">
      <b-card-group deck>
        <!----Breakfast Burrito ----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Breakfast/Breakfast-Burritos-10.jpg"
          img-alt="Breakfast Burrito"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Breakfast Burrito</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.50</b-card-sub-title>
          <b-card-text>Egg, cheese, potatoes, bacon, and hashbrown.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Chile relleno -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Breakfast/chile-rellenos.jpg"
          img-alt="Chile relleno"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chile relleno</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$12.50</b-card-sub-title>
          <b-card-text>Pueblo's poblano pepper stuffed with melted cheese, queso Oaxaca. 
              The stuffed pepper is then covered in an egg white batter, simply corn masa flour and fried.
          </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Chorizo Burrito-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Breakfast/Chorizo-Burrito.jpg"
          img-alt="Chorizo Burrito"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chorizo Burrito</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$9.95</b-card-sub-title>
          <b-card-text>Egg, cheese, potatoes, and chorizo.</b-card-text>
            
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
      </section>
        </b-tab>
        </b-tabs>
    </b-card>
  </div>
<!------------END OF BREAKFAST TAB------------------------------------------------>
  </div>
  </main>
</template>