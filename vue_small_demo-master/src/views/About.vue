<template>
  <div id="app">
    <v-app>
      <v-content>
        <v-container fluid>
          <v-row id="main">
             <v-col id="pic" cols="12" md="7">
               <div id="picbox"><img src="../assets/1.jpg" height="800px" id="img1"></div>
               <div id="infobox1"><br><br><b>PRODUCT DETAILS</b><br><br>

                 <i>Umbrella by DROP.<br>
                   <br>For unpredictable weather conditions<br>
                   <br>Lightweight canopy<br>
                   <br>Heart print<br>
                   <br>Flexible frame to enhance wind resistance<br>
                   <br>Retractable handle<br>
                   <br>Wrist strap<br>
                   <br>Comes with a matching case<br>
                   <br>Compact size</i></div>
             </v-col>

            <v-col id="info" cols="12" md="5">
              <div id="pricebox">
                <i><b>DROP Umbrella</b></i>
                <br><b>DKK 145</b><br><b>Colour: Blue</b><br><br>
                <v-btn id="add"> ADD TO CART </v-btn>
              </div>
              <div id="infobox2">
                <br><br><b>SIZE & FIT</b><br>

                <br>Measurements when closed: H: 22cm/9" W: 5cm/2"
                <br>Measurements when open: 86cm/34"

                <br><br><b>LOOK AFTER ME</b>

                <br><br>Just here for the care instructions?
                <br>We've got you covered
                <br>Wipe Clean with a damp cloth or sponge

                <br><br><b>ABOUT ME</b>

                <br>Main: 100% Polyester.
              </div>
            </v-col>
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
        </v-container>
      </v-content>
    </v-app>
  </div>
</template>

<style>

  #main {
    color:black;

  }
  #img1{

    border-radius: 30px 150px 75px;
  }
  #pic{


  }
  #footer {
    background-color: black;
    color: white;
    height: 125px;
  }
  #picbox {
    background-color: white;
    border:2px solid black;
    border-radius: 30px 150px 75px;
    margin: 0 auto;

  }
  #infobox1 {
    background-color:white;
    width: 400px;
    height: 650px;
    border:2px solid black;
    border-radius: 15px 50px 30px;
    margin: 0 auto;
    font-size: 18px;
  }
  #pricebox {
    background-color:white;
    height: 800px;
    width: 800px;
    text-align: left;
    display: flex;
    flex-flow: column;
    padding: 200px;
    font-size: 36px;
    border:2px solid black;
    border-radius: 30px 150px 75px;
    margin: 0 auto;
  }
  #add {
   background-color: black;
    color: white;
  }
  #infobox2 {
    background-color:white;
    height: 650px;
    width: 650px;
    font-size: 26px;
    border:2px solid black;
    border-radius: 15px 100px 50px;
    margin: 0 auto
  }

</style>