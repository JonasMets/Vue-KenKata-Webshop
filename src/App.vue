<template>
  <div id="app">
    
    <Header1></Header1>

    <!-- här visas den view som är vald i router -->
    <router-view/>

  </div>
</template>


<script>
// import Navbar from "@/components/navigation/Navbar";
import Header1 from "@/components/header/Header1";

export default {
  components: {
    //
    Header1
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');


/*  här lägger vi de färger som ska användas */
:root{
  --primaryColor:#20D3C2;
  --primaryColorDarker:#1eafa0;

  --mediumGrey: #8A8A8A;
  --almostBlack: #333333;

  --inputField: #FBFBFB;

  --lightPink: #FDF3D7;

}

.font-roboto{
  font-family:'Roboto', sans-serif !important;
  font-size: 16px !important;
}

/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
} */

/* #nav {
  padding: 30px;
} */

/* #nav a {
  font-weight: bold;
  color: #2c3e50;
} */

/* #nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
