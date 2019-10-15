<template>
    <div id="nav">
        <div class="nav_container">
            <div class="leftSide">
                <div class="logo">
                    DROP.
                </div>
                <div class="nav_wrapper">
                    <div class="socials"><router-link to="/about" class="routerLink"><i class="fas fa-shopping-cart"/></router-link></div>
                    <div class="socials"><router-link to="/" class="routerLink"><i class="fas fa-home"/></router-link></div>
                </div>
            </div>
            <div class="icons">
                <div class="socials_container">
                    <div class="socials"><i class="fab fa-instagram"></i></div>
                    <div class="socials"><i class="fab fa-facebook"></i></div>
                    <div class="socials"><i class="fab fa-youtube"></i></div>
                </div>

            </div>
        </div>
        <div class="logo_bar">
            <img src="../assets/72122682_483140439206927_1006645943686135808_n.png" height="250" >
        </div>
    </div>
</template>

<script>
    export default {
        name: "NavBar"
    }
</script>

<style scoped>
    .routerLink{
        color: white;
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
        border: 0px solid white;
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
    .socials:hover{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
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