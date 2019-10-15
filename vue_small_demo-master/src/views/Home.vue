<template>
  <div id="app">
    <NavBar/>
    <v-app>
      <v-content>
        <v-container id="vcon" fluid>
          <v-row id="main">
            <v-col id="maincol" >
              <v-row id="maintop">

                <v-carousel height="800px" id="carousel">
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
                <v-col cols="12" md="4"><v-hover id="hover1"
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard1"
                          :elevation="hover ? 12 : 2"
                          height="750"
                          class="mx-auto"
                          max-width="600px"
                          onclick="location.href = '/about'"
                  >


                    <v-img
                            class="black--text"
                            height="600px"
                            src="../assets/1.jpg"
                    >
                      <v-card-title class="align-end fill-height"></v-card-title>
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
                <v-col cols="12" md="4"><v-hover id="hover2"
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard2"
                          :elevation="hover ? 12 : 2"
                          height="750"
                          class="mx-auto"
                          max-width="600px"
                          onclick="location.href = '/about2'"
                  >


                    <v-img
                            class="black--text"
                            height="600px"
                            src="../assets/2.jpg"
                    >
                      <v-card-title class="align-end fill-height"></v-card-title>
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
                <v-col cols="12" md="4"><v-hover id="hover3"
                        v-slot:default="{ hover }"
                        :open-delay="openDelay"
                        :close-delay="closeDelay"
                        :disabled="disabled"
                        :value="value"
                >
                  <v-card id="vcard3"
                          :elevation="hover ? 12 : 2"
                          height="750"
                          class="mx-auto"
                          max-width="600px"
                          onclick="location.href = '/about3'"
                  >


                    <v-img
                            class="black--text"
                            height="600px"
                            src="../assets/3.jpg"
                    >
                      <v-card-title class="align-end fill-height"></v-card-title>
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
              <v-row>
                <v-hover id="hovervid"
                         v-slot:default="{ hover }"
                         :open-delay="openDelay"
                         :close-delay="closeDelay"
                         :disabled="disabled"
                         :value="value"
                >
                <iframe width="1280" height="720" id="video"
                        :elevation="hover ? 12 : 2"
                        src="https://www.youtube.com/embed/CvBfHwUxHIk">
                </iframe></v-hover>
              </v-row>

            <v-row id="footer">
              <v-col><br>
                <strong><b>Contact Us</b></strong>
                <br>Phone: XX XX XX XX<br>
                Fax: XX XX XX XX<br>

              </v-col>
              <v-col><v-card
              width="100%"
              class="black lighten-1 text-center">
                <v-card-text class="white--text">
                  {{ new Date().getFullYear() }} — <strong><i>DROP</i></strong>
                </v-card-text>
              </v-card></v-col>
              <v-col><i><br>Umbrella DROP is a registered trademark.
                <br>All rights reserved.</i></v-col>
            </v-row>
            </v-col>

           </v-row>
        </v-container>
      </v-content>
    </v-app>
  </div>
</template>

<script>
  import NavBar from './NavBar'
  export default {
      name: "Home",
      components: {
        NavBar
      },
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
  #hovervid{
    opacity: 0.9;
    transition: 0.3s;
    margin: 0 auto;
    margin-bottom: 300px;
  }
  #hovervid:hover {opacity: 1}

  #video{
    margin: 0 auto;
    margin-bottom: 400px;
  }
  #footer {
    background-color: black;
    color: white;
    height: 125px;
  }
  #vcon {
    padding: 0px;

  }
  #maincol {
    padding: 0px;
  }
    #carousel {
    border: black solid;
    border-width: 2px;
    }

  #hover1, #hover2, #hover3, #hover4, #hover5, #hover6 {
      opacity: 0.9;
      transition: 0.3s;
  }

  #hover1:hover {opacity: 1}
  #hover2:hover {opacity: 1}
  #hover3:hover {opacity: 1}
  #hover4:hover {opacity: 1}
  #hover5:hover {opacity: 1}
  #hover6:hover {opacity: 1}

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
    margin-bottom: 100px;
  }
</style>

