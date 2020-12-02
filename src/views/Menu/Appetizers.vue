<template>
  <main role="main">
  <div class="appetizers">
    <!----<h1>This is an about page</h1>--->
    <!----------row 1 : APPETIZERS--------------->
    <div>
    <b-card no-body>
     <b-tabs pills card horizontal id="pills-card-tab">
      <b-tab title="Appetizers" active>

      <section role="region">
      <div class="mt-3">
      <b-card-group deck>
        <!----Rey de nachos----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/rey de nachos.jpg"
          img-alt="Rey de nachos"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Rey De Nachos</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$12.25</b-card-sub-title>
          <b-card-text>Choices: picadillo beef, carnitas, shredded beef or chicken.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Shrimp Cocktail Gigante  -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/shrimp-cocktail-4.jpg"
          img-alt="Shrimp Cocktail Gigante"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Shrimp Cocktail Gigante </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.00</b-card-sub-title>
           <b-card-text>Jumbo size shrimp in a cocktail sauce, chamoy, avocado slices.</b-card-text>
        </b-card-body>
        </b-card>
       <!--------Guacamole & Corn Tortilla Chips  -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/Guacamole-chips.jpg"
          img-alt="Guacamole & Corn Tortilla Chips"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Guacamole & Chips </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.00</b-card-sub-title>
          <b-card-text>Corn-tortilla chips and freshly made guacamole. </b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
      </section>
      
  <!------------row 2: appetizers ------------------------>
      <section role="region">
       <div class="mt-3">
      <b-card-group deck>
        <!----Chicken Tenders ----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/chicken-strips.jpg"
          img-alt="Chicken Tenders"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chicken Tenders</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$11.25</b-card-sub-title>
          <b-card-text>Breaded cage-free chicken strips, cooked to a golden crisp
                  with a serving of ranch, blue cheese, buffalo ranch, or
                  ketcup. Served with celery sticks.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Baked Spinach & Artichoke Dip -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/Baked Spinach & Artichoke Dip.jpg"
          img-alt="Baked Spinach & Artichoke Dip"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Baked Spinach & Artichoke Dip </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.50</b-card-sub-title>
          <b-card-text>With Parmesan, Jack and cream cheeses beneath a crunchy bread
                  crumb topping, served hot in its own skillet with corn
                  tortilla chips. </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Cheese Quesadilla -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/cheese-quesadillas.jpg"
          img-alt="Cheese Quesadilla"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Cheese Quesadilla  </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$12.25</b-card-sub-title>
          <b-card-text>Flour tortilla with a hint of garlic butter and melted jack cheese.
               </b-card-text>
            <b-card-text>Add shredded chicken +$1.00 or shredded beef +$2.00. </b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
        </section>
        </b-tab>
<!------------END OF APPETIZERS TAB------------------------------------------------>


<!---------------SALADS TAB----------------------------------------->
     <b-tab title="Salads">
       <section role="region">
      <div class="mt-3">
      <b-card-group deck>
        <!----Mexican Caesar Grilled Chicken----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/mexican-caesar-salad.jpg"
          img-alt="Mexican Caesar Grilled Chicken"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Mexican Caesar Grilled Chicken</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.25</b-card-sub-title>
          <b-card-text>Romaine lettuce, house-made creamy cilantro caesar, 
              garlic bread, and crispy tortilla strips.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Caesar Salad -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/caesar-salad-plate.jpg"
          img-alt="Caesar Salad"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Caesar Salad </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$12.00</b-card-sub-title>
           <b-card-text> Hand-chopped romaine tossed in-house Caesar dressing with
                  croutons and shaved Parmesan cheese. </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Santa Fe Chicken Salad -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/santa-fe-chicken-salad.jpg"
          img-alt="Santa Fe Chicken Salad"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Santa Fe Chicken Salad </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$14.00</b-card-sub-title>
          <b-card-text>Spicy grilled chicken, black beans, avocado, corn, tomatoe cherries, cilantro, tortilla
                  strips, house-made ranch & a drizzle of spicy Santa Fe sauce.</b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
       </section>
        </b-tab>

<!---------------END OF THE SALADS TAB------------------------------------->

<!---------------SOUPS TAB----------------------------------------->
     <b-tab title="Soups">
      <section role="region">
      <div class="mt-3">
      <b-card-group deck>
        <!----Menudo----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/Menudo.jpg"
          img-alt="Menudo"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Menudo</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.25</b-card-sub-title>
          <b-card-text>Beef tripe soup. Served with a side of cilantro, jalepanos, 
              onions, radishes, lime, cabbage, and corn tortillas.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Pozole-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/pozole.jpg"
          img-alt="Pozole"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Pozole </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$12.75</b-card-sub-title>
           <b-card-text>Pork with homeny. Served with a side of cilantro, jalepanos, 
              onions, radishes, lime, cabbage, and corn tortillas. </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Loaded Potato Soup-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/loaded-baked-potato-soup.jpg"
          img-alt="Loaded Potato Soup"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Loaded Potato Soup </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$10.00</b-card-sub-title>
          <b-card-text>Topped with bacon, cheddar and fresh green onions. Served in a
                  bowl.</b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
      </section>

       <section role="region">
      <div class="mt-3">
      <b-card-group deck>
        <!----Chicken Soup----------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/Chicken-Rice-Soup.jpg"
          img-alt="Chicken Soup"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chicken Soup</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.25</b-card-sub-title>
          <b-card-text>A soup simmered in water and chicken broth, with chicken, noodles, vegetables, rice, barley.</b-card-text>
        </b-card-body>
        </b-card>

      <!--------Beef Soup -------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/vegetable-beef-soup.jpg"
          img-alt="Beef Soup"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Beef Soup </b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$13.75</b-card-sub-title>
           <b-card-text>A soup simmered in water and bef broth, with beef, 
               potatoes, and vegetables.
                </b-card-text>
        </b-card-body>
        </b-card>
       <!--------Chicken Tortilla Soup-------------->
       <b-card
          no-body
          style="max-width: 40rem;"
          img-src="../../assets/Appetizers/chicken-tortilla-soup.jpg"
          img-alt="Chicken Tortilla Soup"
          img-top
        >
        <b-card-body>
          <b-card-title id="title"><b>Chicken Tortilla Soup</b></b-card-title>
          <b-card-sub-title class="mb-2" id="price">$14.00</b-card-sub-title>
          <b-card-text> Chicken breast in a seasoned broth, topped with Monterey Jack
                  and Cheddar cheese, cilantro and crispy tortilla strips.
                  Served with a wedge of lime.</b-card-text>
        </b-card-body>
        </b-card>
         </b-card-group>
        </div>
       </section>
        </b-tab>

<!---------------END OF THE SOUPS TAB------------------------------------->

    </b-tabs>
    </b-card>
  </div>
  </div>
  </main>
</template>