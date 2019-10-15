<template>
  <div id="app">
    <div>
    <router-view/>
  </div>
  </div>
</template>

<script>
  export default {
    name: "App",
    components: {
    }
  };
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    min-height: 100vh;
  }
  .routerLink{
    color: white;
  }
  body, html{
    padding: 0;
    margin: 0;
    background-size: cover;
    background: gray;
  }
  .invert{
    filter: invert(100%);
  }
  .nav_container{
    height: 60px;
    width: 100%;
    display: flex;
  }
  .leftSide{
    width: 50%;
    height: 60px;
    font-size: 50px;
    background: black;
    font-family: myFirstFont;
    color: white;
    display: flex;
    align-items: center;
    padding: 0px 10px 0px 20px;
    border: white solid;
    border-width: 0px 0px 0px 0px;
    justify-content: space-between;
  }
  .logo{
    display: flex;
    align-items: center;

  }
  .icons{
    width: 50%;
    display: flex;
    justify-content: flex-end;
    font-size: 30px;
    color: black;
    background-color: white;
    border: black solid;
    border-width: 0px 0px 2px 0px;
  }
  .nav_wrapper{
    width:150px;
    height: 60px;
    font-size: 30px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
  }
  .socials:hover {
    transform: skewY(25deg);
  }
  .logo:hover {
    transform: rotate3d(1, 1, 1, 17deg);
    transition-duration: 1.3s;
  }
  .imglogo:hover {
    transform: rotate(360deg);
    transition-duration: 2s;
  }

  .socials_container{
    width: 200px;
    height: 60px;
    display: flex;
    justify-content: space-around;
    align-items: center;;
  }
  .logo_bar {
    justify-content: center;
    background: white;
    display: flex;
    height: 300px;
    align-items: center;
  }
</style>
