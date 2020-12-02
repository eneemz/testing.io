<template>
  <main role="main">
    <div class="drinks">
      <!----<h1>This is an drinks page</h1>--->
      <!----------row 1 : Non-alcholic drinks--------------->
      <div>
        <b-card no-body>
          <b-tabs pills card horizontal id="pills-card-tab">
            <b-tab title="Non-alcoholic Beverages" active id="non-al-drinks">
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Soda----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/soda.jpg"
                      img-alt="Soda"
                      img-top
                    >
                      <b-card-body id="soda-card">
                        <b-card-title id="title"><b>Soda</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$2.50</b-card-sub-title
                        >
                        <b-card-text>
                          Choices: Pepsi, Coca-cola, Diet Coca-cola, Sprite,
                          Mountain Dew, Dr. Pepper, or Root Beer.</b-card-text
                        >
                      </b-card-body>
                    </b-card>

                    <!--------Juice -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/juices.jpg"
                      img-alt="Juice"
                      img-top
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Juice </b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$3.00</b-card-sub-title
                        >
                        <b-card-text
                          >Choices: Apple, pineapple, mango, kiwi, orange,
                          cranberry, or grapefruit.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                    <!--------Lemonade -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/lemonade_v3.jpg"
                      img-alt="Lemonade"
                      img-top
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Lemonade </b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$3.00</b-card-sub-title
                        >
                        <b-card-text
                          >Choices: plain lemonade or strawberry lemonade.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>

              <!------------row 2: non-alcholic drinks------------------------>
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Milk ----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/milk.jpg"
                      img-alt="Milk"
                      img-top
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Milk</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$2.25</b-card-sub-title
                        >
                        <b-card-text
                          >Choices: 2% Milk, Fat-free Milk, or Soy Milk ($3.50).
                        </b-card-text>
                      </b-card-body>
                    </b-card>

                    <!--------Coffee -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/coffee.jpg"
                      img-alt="Coffee"
                      img-top
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Coffee </b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$2.50</b-card-sub-title
                        >
                        <b-card-text>Choices: Decafe or regular. </b-card-text>
                      </b-card-body>
                    </b-card>
                    <!--------Tea -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/a-cup-of-tea.jpg"
                      img-alt="Tea"
                      img-top
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Tea </b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$3.25</b-card-sub-title
                        >
                        <b-card-text
                          >Choices: Mango Iced Tea, Blackberry Iced Tea, Half
                          Tea | Half Lemonade, or Unsweetened Tea.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
            </b-tab>
            <!------------END OF NON ALCOHOLIC DRINKS TAB------------------------------------------------>

            <!----------row 1 : Beer drinks--------------->
            <b-tab title="Beer">
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Bud Light----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/bud-light_v2.jpg"
                      img-alt="Bud Light"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Bud Light</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.75</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>

                    <!--------Coors Light-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/coors-light_v3.jpg"
                      img-alt="Coors Light"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Coors Light</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Corona Light-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Corona-Light.png"
                      img-alt="Corona Light"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Corona Light</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>

              <!----------row 2 : Beer drinks--------------->
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!--------Budweiser-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/budweiser.jpg"
                      img-alt="Budweiser"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Budweiser</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Blue Moon-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/blue-moon.jpg"
                      img-alt="Blue Moon"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Blue Moon</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Corona Extra-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/corona-extra.jpg"
                      img-alt="Corona Extra"
                      img-top
                      id="image-corona-extra"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Corona Extra</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
              <!----------row 3 : Beer drinks--------------->
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!--------Heineken-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Heineken.png"
                      img-alt="Heineken"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Heineken</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Estrella Jalisco-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/estrella-jalisco.png"
                      img-alt="Estrella Jalisco"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Estrella Jalisco</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.50</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>

                    <!-----Dos Equis----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/dos-equis.jpg"
                      img-alt="Dos Equis"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"><b>Dos Equis</b></b-card-title>
                        <b-card-sub-title class="mb-2" id="price"
                          >$5.00</b-card-sub-title
                        >
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
            </b-tab>
            <!------------END OF BEERS  TAB------------------------------------------------>

            <!----------row 1 : Red Wine drinks--------------->
            <b-tab title="Red Wine">
              <b-card-text
                >*The sizes of all the red wine bottles are 750 ml.
              </b-card-text>
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Michael Pozzan Merlot----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Michael-Pozzan-Merlot.jpg"
                      img-alt="Michael Pozzan Merlot"
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="michael-pozzan-merlot-card">
                        <b-card-title id="title"
                          ><b>Michael Pozzan Merlot</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$27.85</b-card-sub-title
                        >
                        <b-card-text
                          >Napa County, California. Dark raspberry aromas on the
                          nose followed by a firm tannic structure where the
                          earthy notes add depth to the cherry and herb
                          flavors.</b-card-text
                        >
                      </b-card-body>
                    </b-card>

                    <!--------Pedroncelli Zinfandel Mother Clone -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Pedroncelli Zinfandel Mother Clone.jpg"
                      img-alt="Pedroncelli Zinfandel Mother Clone"
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="pedroncelli-zinfandel-mother-clone-card">
                        <b-card-title id="title"
                          ><b
                            >Pedroncelli Zinfandel Mother Clone
                          </b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$12.95</b-card-sub-title
                        >
                        <b-card-text
                          >Pedroncelli Winery & Vineyards, California. Fragrant aroma of
                          raspberry and red plum with a touch of black pepper
                          and vanilla.</b-card-text
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Firestone Merlot, Santa Ynez -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Firestone Merlot, Santa Ynez.jpg"
                      img-alt="Firestone Merlot, Santa Ynez"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Firestone Merlot, Santa Ynez </b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$18.78</b-card-sub-title
                        >
                        <b-card-text
                          >Santa Barbara County, California. Medium to deep ruby
                          color; showy, ripe fruit aroma; medium bodied, firm
                          and textured on the palate; bright red fruit flavors.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
              <!----------row 2 : Red Wine drinks--------------->
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Menage a Trois Red----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Menage a Trois Red.jpg"
                      img-alt="Menage a Trios Red"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Menage a Trois Red</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$10.49</b-card-sub-title
                        >
                        <b-card-text
                          >Folie a Deux Winery, California. Menage a Trois Red
                          is soft and pleasing red wine; easy on the palate; a
                          really tasty, cocktail type of red wine.</b-card-text
                        >
                      </b-card-body>
                    </b-card>

                    <!--------Bogle Vineyard Zinfandel -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Bogle Vineyards Zinfandel.jpg"
                      img-alt="Bogle Vineyward Zinfandel "
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="bogle-vineyard-zinfandel-card">
                        <b-card-title id="title"
                          ><b>Bogle Vineyard Zinfandel</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$13.45</b-card-sub-title
                        >
                        <b-card-text
                          >Bogle Vineyards, California. Jammy with sturdy
                          structure saturated with dark fruit with hints of
                          lavender & savory herbs.</b-card-text
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Monte Antico Rosso -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Monte Antico Rosso.jpg"
                      img-alt="Monte Antico Rosso"
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="monte-antico-rosso-card">
                        <b-card-title id="title"
                          ><b>Monte Antico Rosso</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$17.64</b-card-sub-title
                        >
                        <b-card-text
                          >Tuscany, Italy. It's a fruity wine
                          black cherry, blueberry, and hints of pepper; full and
                          velvety with a long and delicious finish.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
            </b-tab>
            <!------------END OF RED WINE TAB------------------------------------------------>

            <!----------row 1 : White Wine drinks--------------->
            <b-tab title="White Wine">
              <b-card-text
                >*The sizes of all the white wine bottles are 750 ml.
              </b-card-text>
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Kendall-Jackson Chardonnay Vintner's Reserve----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Kendall-Jackson Chardonnay Vintner's Reserve.jpg"
                      img-alt="Kendall-Jackson Chardonnay Vintner's Reserve"
                      img-top
                      id="image-card"
                    >
                      <b-card-body
                        id="kendall-jackson-chardonnay-vintners-reserve-card"
                      >
                        <b-card-title id="title"
                          ><b
                            >Kendall-Jackson Chardonnay Vintner's Reserve</b
                          ></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$13.65</b-card-sub-title
                        >
                        <b-card-text
                          >Kendall-Jackson Winery, California. Fruity, smooth
                          and slightly spicy, this medium-bodied wine is a
                          crowd-pleaser.</b-card-text
                        >
                      </b-card-body>
                    </b-card>

                    <!--------Pine Ridge Chenin Blanc-Viognier -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Pine Ridge Chenin Blanc-Viognier.jpg"
                      img-alt="Pine Ridge Chenin Blanc-Viognier "
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="pine-ridge-chenin-blanc-viognier-card"> 
                        <b-card-title id="title"
                          ><b>Pine Ridge Chenin Blanc-Viognier</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$20.34</b-card-sub-title
                        >
                        <b-card-text
                          >Pine Ridge Windery, California. Brilliant and
                          refreshing; a delightful array of lemongrass, honeydew
                          and sweet tropical aromas; crisp and mouthwatering on
                          the palate.</b-card-text
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Cantina di Casteggio Moscato -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Cantina di Casteggio Moscato.jpg"
                      img-alt="Cantina di Casteggio Moscato"
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="cantina-di-casteggio-moscato-card">
                        <b-card-title id="title"
                          ><b>Cantina di Casteggio Moscato </b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$18.14</b-card-sub-title
                        >
                        <b-card-text
                          >Lombardy, Italy. Aromatic and delicate the delightful
                          Cantina di Casteggio Moscato is fresh and easy; fun
                          with flowers and ripe peaches; sweet, with fine
                          balance.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
              <!----------row 2 : White Wine drinks--------------->
              <section role="region">
                <div class="mt-3">
                  <b-card-group deck>
                    <!----Fetzer Gewurztraminer----------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Fetzer Gewurztraminer .jpg"
                      img-alt="Fetzer Gewurztraminer"
                      img-top
                      id="image-card"
                    >
                      <b-card-body>
                        <b-card-title id="title"
                          ><b>Fetzer Gewurztraminer</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$8.27</b-card-sub-title
                        >
                        <b-card-text
                          >Fetzer Winery, California. Complex aromas of
                          tangerine, mango and orange spice. Rich flavors of
                          pineapple, baked pears, cinnamon, clove and
                          caramelized apples.</b-card-text
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Maddalena Vineyards Riesling -------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Maddalena Vineyards Riesling.jpg"
                      img-alt="Maddalena Vineyards Riesling"
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="maddalena-vineyards-riesling-card">
                        <b-card-title id="title"
                          ><b>Maddalena Vineyards Riesling</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$15.05</b-card-sub-title
                        >
                        <b-card-text
                          >Monterey County, California. It greets the palate
                          with fresh fruit flavors of pear & green apple. It
                          balances natural acidity and sweetness.</b-card-text
                        >
                      </b-card-body>
                    </b-card>
                    <!--------Henderson Trail Pinot Gris-------------->
                    <b-card
                      no-body
                      style="max-width: 40rem;"
                      img-src="../../assets/Drinks/Henderson Trail Pinot Gris.jpg"
                      img-alt="Henderson Trail Pinot Gris"
                      img-top
                      id="image-card"
                    >
                      <b-card-body id="henderson-trail-pinot-gris-card">
                        <b-card-title id="title"
                          ><b>Henderson Trail Pinot Gris</b></b-card-title
                        >
                        <b-card-sub-title class="mb-2" id="price"
                          >$24.58</b-card-sub-title
                        >
                        <b-card-text
                          >Willamette Valley, Oregon. Aromas of mineral, slate,
                          white peach, oranges, vanilla; the palate is
                          lively & focused w/ apple, pear, key lime, & honey
                          suckle.
                        </b-card-text>
                      </b-card-body>
                    </b-card>
                  </b-card-group>
                </div>
              </section>
            </b-tab>
            <!------------END OF WHITE WINE TAB------------------------------------------------>
          </b-tabs>
        </b-card>
      </div>
    </div>
  </main>
</template>

<style scoped>
#pedroncelli-zinfandel-mother-clone-card{
  height: 175px;
}
#michael-pozzan-merlot-card{
  height: 175px;
}
#monte-antico-rosso-card{
  height: 175px;
}
#bogle-vineyard-zinfandel-card{
  height: 175px;
}
#henderson-trail-pinot-gris-card{
  height: 175px;
}
#pine-ridge-chenin-blanc-viognier-card{
  height: 220px;
}
#kendall-jackson-chardonnay-vintners-reserve-card, #cantina-di-casteggio-moscato-card{
  height: 220px;
}
#soda-card{
  height: 100px;
}
</style>
<!---<style>
#soda-card{
  height: 50px;
}

#michael-pozzan-merlot-card{
  height: 220px;
}

#bogle-vineyard-zinfandel-card{
  height: 195px;
}

#maddalena-vineyards-riesling-card{
  height: 195px;
}

#kendall-jackson-chardonnay-vintners-reserve-card, #cantina-di-casteggio-moscato-card{
  height: 270px;
}
</style>--->
