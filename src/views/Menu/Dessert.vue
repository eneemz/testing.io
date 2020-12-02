<template>
  <main role="main">
  <div class="dessert">
    <div>
    <b-card no-body>
      <b-tabs pills card horizontal id="pills-card-tab">
         <b-tab title="Dessert" active id="dessert">
    <!----------row 1--------------->
    <section role="region">
    <div class="mt-3">
      <!---Skillet Chocolate Chip cookie-->
      <b-card-group deck>
   
        <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dessert/Chocolate-Chip-Skillet-Cookie-Landscape.jpg"
          img-alt="Skillet Chocolate Chip Skillet"
          img-top
        >  
        <b-card-body>
          <b-card-title id="title"><b>Skillet Chocolate Chip Cookie</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$7.50</b-card-sub-title>
          <b-card-text>
           Topped with vanilla ice cream and hot fudge.
          </b-card-text>
        </b-card-body>
        </b-card>

      <!------Molten Chocolate Cake---------->
        <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dessert/molten-choco-cake.jpg"
          img-alt="Molten Chocolate Cake"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Molten Chocolate Cake</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$7.75</b-card-sub-title>
          <b-card-text>
            Chocolate cake with a molten chocolate center, topped with
            vanilla ice cream in a chocolate shell.
          </b-card-text>
        </b-card-body>
        </b-card>

      <!-------Ice Cream----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dessert/chocolate-peanut-butter-cup-ice-cream-3-550.jpg"
          img-alt="Ice cream"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Ice cream</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$6.00</b-card-sub-title>
          <b-card-text>
            Vanilla, strawberry, chocolate, chocolate chip, or
             rocky road. Served in a bowl.
          </b-card-text>
        </b-card-body>
        </b-card>
      </b-card-group>
    </div>
    </section>

<!----------row 2--------------->
<section role="region">
    <div class="mt-3">
      <b-card-group deck>
        <!----Flan----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dessert/flan.jpg"
          img-alt="Flan"
          img-top
        >
        <b-card-body id="flan-card"> 
          <b-card-title id="title"><b>Flan</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$5.25</b-card-sub-title>
          <b-card-text>
            A round, sponge-cake pastry coated with sweet syrup.
          </b-card-text>
        </b-card-body>
        </b-card>

      <!--------tres leche cake-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dessert/Tres-Leches-Cake-Recipe-6.jpg"
          img-alt="Tres leches cake"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Tres leches cake</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$5.50</b-card-sub-title>
          <b-card-text>
            A sponge cake with whipped cream and sliced strawberries on top.
          </b-card-text>
        </b-card-body>
        </b-card>


      <!-----Churros----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Dessert/Churros_9-SQ.jpg"
          img-alt="Churros"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Churros</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$8.00 / 12 pc</b-card-sub-title>
          <b-card-text>
           Fried-dough pastry served with a cup of chocolate dipping sauce.
          </b-card-text>
        </b-card-body>
        </b-card>
      </b-card-group>
    </div>
    </section>
     </b-tab>
    </b-tabs>
    </b-card>
    </div>
    


  </div>
  </main>
</template>

