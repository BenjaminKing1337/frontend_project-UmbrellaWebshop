<template>
  <div id="app">
    <v-app>
      <v-content>
        <v-container id="vcon" fluid>
          <v-row id="main">
            <v-col id="maincol" >
              <v-row id="maintop">

                <v-carousel>
                  <v-carousel-item
                          v-for="(item,i) in items"
                          :key="i"
                          :src="item.src"
                          reverse-transition="fade-transition"
                          transition="fade-transition"
                  ></v-carousel-item>
                </v-carousel>
              </v-row>
              <v-row id="mainmid">
                <v-col cols="12" md="12">

                </v-col>
              </v-row>
              <v-row id="mainbot">
                <v-col cols="12" md="4"><v-hover
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="550"
                          class="mx-auto"
                          max-width="600px"
                  >


                    <v-img
                            class="black--text"
                            height="400px"
                            src="https://cdn.shopify.com/s/files/1/0727/4975/products/Big_Umbrella_LifeTek_Hillcrest_Golf_Umbrella_2048x.jpg?v=1520618406"
                    >
                      <v-card-title class="align-end fill-height">Umbrella</v-card-title>
                    </v-img>

                    <v-card-text>
                      <span>Price: Money</span><br>
                      <span class="text--primary">
                    <span>Good for rain!</span><br>
                    <span>Timeless design assures absolute satisfaction</span>
                  </span>
                    </v-card-text>

                    <v-card-actions>
                      <v-btn
                              text
                              color="black"
                      >
                        Add to Cart
                      </v-btn>
                      <v-btn
                              text
                              color="black"
                      >
                        Buy Now
                      </v-btn></v-card-actions></v-card></v-hover></v-col>
                <v-col cols="12" md="4"><v-hover
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="550"
                          class="mx-auto"
                          max-width="600px"
                  >


                    <v-img
                            class="black--text"
                            height="400px"
                            src="https://cdn.shopify.com/s/files/1/0727/4975/products/Big_Umbrella_LifeTek_Hillcrest_Golf_Umbrella_2048x.jpg?v=1520618406"
                    >
                      <v-card-title class="align-end fill-height">Umbrella</v-card-title>
                    </v-img>

                    <v-card-text>
                      <span>Price: Money</span><br>
                      <span class="text--primary">
                    <span>Good for rain!</span><br>
                    <span>Timeless design assures absolute satisfaction</span>
                  </span>
                    </v-card-text>

                    <v-card-actions>
                      <v-btn
                              text
                              color="black"
                      >
                        Add to Cart
                      </v-btn>
                      <v-btn
                              text
                              color="black"
                      >
                        Buy Now
                      </v-btn></v-card-actions></v-card></v-hover></v-col>
                <v-col cols="12" md="4"><v-hover
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="550"
                          class="mx-auto"
                          max-width="600px"
                  >


                    <v-img
                            class="black--text"
                            height="400px"
                            src="https://cdn.shopify.com/s/files/1/0727/4975/products/Big_Umbrella_LifeTek_Hillcrest_Golf_Umbrella_2048x.jpg?v=1520618406"
                    >
                      <v-card-title class="align-end fill-height">Umbrella</v-card-title>
                    </v-img>

                    <v-card-text>
                      <span>Price: Money</span><br>
                      <span class="text--primary">
                    <span>Good for rain!</span><br>
                    <span>Timeless design assures absolute satisfaction</span>
                  </span>
                    </v-card-text>

                    <v-card-actions>
                      <v-btn
                              text
                              color="black"
                      >
                        Add to Cart
                      </v-btn>
                      <v-btn
                              text
                              color="black"
                      >
                        Buy Now
                      </v-btn></v-card-actions></v-card></v-hover></v-col>
                <v-col cols="12" md="4"><v-hover
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="550"
                          class="mx-auto"
                          max-width="600px"
                  >


                    <v-img
                            class="black--text"
                            height="400px"
                            src="https://cdn.shopify.com/s/files/1/0727/4975/products/Big_Umbrella_LifeTek_Hillcrest_Golf_Umbrella_2048x.jpg?v=1520618406"
                    >
                      <v-card-title class="align-end fill-height">Umbrella</v-card-title>
                    </v-img>

                    <v-card-text>
                      <span>Price: Money</span><br>
                      <span class="text--primary">
                    <span>Good for rain!</span><br>
                    <span>Timeless design assures absolute satisfaction</span>
                  </span>
                    </v-card-text>

                    <v-card-actions>
                      <v-btn
                              text
                              color="black"
                      >
                        Add to Cart
                      </v-btn>
                      <v-btn
                              text
                              color="black"
                      >
                        Buy Now
                      </v-btn></v-card-actions></v-card></v-hover></v-col>
                <v-col cols="12" md="4"><v-hover
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="550"
                          class="mx-auto"
                          max-width="600px"
                  >


                    <v-img
                            class="black--text"
                            height="400px"
                            src="https://cdn.shopify.com/s/files/1/0727/4975/products/Big_Umbrella_LifeTek_Hillcrest_Golf_Umbrella_2048x.jpg?v=1520618406"
                    >
                      <v-card-title class="align-end fill-height">Umbrella</v-card-title>
                    </v-img>

                    <v-card-text>
                      <span>Price: Money</span><br>
                      <span class="text--primary">
                    <span>Good for rain!</span><br>
                    <span>Timeless design assures absolute satisfaction</span>
                  </span>
                    </v-card-text>

                    <v-card-actions>
                      <v-btn
                              text
                              color="black"
                      >
                        Add to Cart
                      </v-btn>
                      <v-btn
                              text
                              color="black"
                      >
                        Buy Now
                      </v-btn></v-card-actions></v-card></v-hover></v-col>
                <v-col cols="12" md="4"><v-hover
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="550"
                          class="mx-auto"
                          max-width="600px"
                  >


                    <v-img
                            class="black--text"
                            height="400px"
                            src="https://cdn.shopify.com/s/files/1/0727/4975/products/Big_Umbrella_LifeTek_Hillcrest_Golf_Umbrella_2048x.jpg?v=1520618406"
                    >
                      <v-card-title class="align-end fill-height">Umbrella</v-card-title>
                    </v-img>

                    <v-card-text>
                      <span>Price: Money</span><br>
                      <span class="text--primary">
                    <span>Good for rain!</span><br>
                    <span>Timeless design assures absolute satisfaction</span>
                  </span>
                    </v-card-text>

                    <v-card-actions>
                      <v-btn
                              text
                              color="black"
                      >
                        Add to Cart
                      </v-btn>
                      <v-btn
                              text
                              color="black"
                      >
                        Buy Now
                      </v-btn></v-card-actions></v-card></v-hover></v-col>
              </v-row>

            <v-row id="footer">
              <v-card
              width="100%"
              class="black lighten-1 text-center">
                <v-card-text class="white--text">
                  {{ new Date().getFullYear() }} — <strong>Umbrella</strong>
                </v-card-text>
              </v-card>
            </v-row>
            </v-col>

           </v-row>
        </v-container>
      </v-content>
    </v-app>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: 'https://www.ikea.com/PIAimages/0711831_PE728510_S5.JPG',
          },
          {
            src: 'https://cdn.shopify.com/s/files/1/1932/8237/products/Blunt-Umbrella-Classic-Under-Navy_1024x1024@2x.png?v=1564147260',
          },
          {
            src: 'https://cache.mrporter.com/variants/images/666467151993456/in/w2000_q80.jpg',
          },
          {
            src: 'https://stumbrellas.co.za/wp-content/uploads/2018/11/st-28-red.png',
          },
        ],
      }
    },
  }
</script>

<style>
  body, html{
  background: gray;
  }
  #vcon {
    background-color:

  }

  #app {
      background-image: url("../assets/backgroundblack.jpg");
      background-repeat: repeat-y;
      background-size: cover;
  }

  #maintop {
    margin-top: 0px;
    background-color: black;
  }
  #mainbot {
    margin-top: 50px;
  }
</style>

