<template>
  <div id="app">
    <!-- header -->
    <Header1></Header1>

    <!-- här visas den view som är vald i router -->
    <router-view />

    



    <!-- footer -->
    <Footer1></Footer1>

  </div>
</template>


<script>
// import Navbar from "@/components/navigation/Navbar";
import Header1 from "@/components/header/Header1";
import Footer1 from "@/components/footer/Footer1";

export default {
  components: {
    //
    Header1,
    Footer1
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap");

/*  här lägger vi de färger som ska användas */
:root {
  --primaryColor: #20d3c2;
  --primaryColorDarker: #1eafa0;

  --mediumGrey: #8a8a8a;
  --almostBlack: #333333;

  --inputField: #fbfbfb;

  --lightPink: #fdf3d7;
}

.font-roboto {
  font-family: "Roboto", sans-serif !important;
  font-size: 16px !important;
}

#app {
  font-family: "Roboto", sans-serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
}

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
