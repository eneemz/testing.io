<template>
  <main role="main">
  <div class="lunch">
    <!---<h1>This is an lunch page</h1>---->
    <div>
    <b-card no-body>
     <b-tabs pills card horizontal id="pills-card-tab">
      <b-tab title="Lunch" active>
          <b-card-text> *All lunch dishes are served with rice, 
              beans, and tortillas--choice of corn or flour.
          </b-card-text>
  <!------------row 1: lunch ------------------------>
     <section role="region">
      <div class="mt-3">
      <b-card-group deck>
        <!----Carne Asada Taco----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Lunch/carne-asada-tacos.jpg"
          img-alt="Carne Asada Taco"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Carne Asada Taco</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.00</b-card-sub-title>
          <b-card-text>Grilled beef taco. Served on the side: cilantro onions, radishes, lime, and red and green sauce.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Sopes -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Lunch/sopes-2-500x500.jpg"
          img-alt="Sopes"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Sopes </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.00</b-card-sub-title>
           <b-card-text>Two homemade thick corn tortillas with shredded chicken or beef, topped 
             with cheese, lettuce, salsa roja, pico de gallo, and sour cream.
               </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Carne Asada Fries -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Lunch/carne-asada-fries.jpg"
          img-alt="Carne Asada Fries"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Carne Asada Fries </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.00</b-card-sub-title>
          <b-card-text>Consists of french fries, pico de gallo, carne asada, guacamole, sour 
            cream, and cheese.</b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
     </section>
      
  <!------------row 2: lunch ------------------------>
      <section role="region">
       <div class="mt-3">
      <b-card-group deck>
        <!----ENCHILADAS RANCHERAS----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Lunch/enchiladas-rancheras.jpg"
          img-alt="Enchiladas Rancheras"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Enchiladas Rancheras</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$14.50</b-card-sub-title>
          <b-card-text>Grilled chicken, jack cheese, tomato, lettuce, salsa ranchera, sour cream, and avocado.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Carne asada and cheese enchilada -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Lunch/CARNE-ASADA-AND-CHEESE-ENCHILADA.jpg"
          img-alt="Carne Asada & Cheese Enchilada"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Carne Asada & Cheese Enchilada </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$12.50</b-card-sub-title>
          <b-card-text>Grilled beef and cheese enchilada, guacamole, and sour cream.
          </b-card-text>
        </b-card-body>
        </b-card>
       <!-------- Steak Molcajete-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Lunch/steak-molcajete.jpg"
          img-alt="Steak Molcajete"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Steak Molcajete</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$16.50</b-card-sub-title>
          <b-card-text>Homemade salsa with grilled nopal and chorizo, monterey jack cheese, grilled 
            cambray onions, avocado.</b-card-text>
            
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