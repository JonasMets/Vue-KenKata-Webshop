<template>
  <div id="app">
    <!-- header -->
    <Header1></Header1>

    <!-- här visas den view som är vald i router -->
    <router-view />

    <!-- brands -->
    <Brand1></Brand1>

    <!-- footer -->
    <Footer1></Footer1>
  </div>
</template>


<script>
// import Navbar from "@/components/navigation/Navbar";
import Header1 from "@/components/header/Header1";
import Footer1 from "@/components/footer/Footer1";
import Brand1 from "@/components/brands/Brand1";

export default {
  components: {
    //
    Header1,
    Footer1,
    Brand1,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap");

/* @import url('https://fonts.googleapis.com/css2?family=Play&display=swap'); */

@import url('https://fonts.googleapis.com/css2?family=Play:wght@400;700&display=swap');

/*  här lägger vi de färger som ska användas */
:root {
  --primaryColor: #20d3c2;
  --primaryColorDarker: #1eafa0;
  /* --primaryColorDark: #080c24; */

  --mydark-blue: #0e153d;

  --white: #ffffff;

  --mediumGrey: #8a8a8a;
  --almostBlack: #333333;

  --inputField: #fbfbfb;

  --lightPink: #fdf3d7;
}

.font-roboto {
  font-family: "Roboto", sans-serif !important;
  font-size: 16px !important;
}
.font-play {
  font-family: 'Play', sans-serif !important;
}

.color-primary {
 color: var(--primaryColor);
}

.my-bg-primary {
  background-color: var(--primaryColor);
}

.my-bg-dark-blue {
  background-color: var(--mydark-blue);
}

.my-bg-dblue-opacity-65 {
    background-color: #0E153D;
    opacity: 0.70;
  }

.my-text-white {
  color: var(--white);
}

#app {
  font-family: "Roboto", sans-serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50; */
}

.fz-14 {
  font-size: 14px !important;
}


.fs-16 {
  font-size: 16px !important;
}

.fs-18 {
  font-size: 18px !important;
}

.fs-24 {
  font-size: 24px !important;
}

.fs-36 {
    font-size: 36px !important;
  }

.fs-60 {
  font-size: 60px !important;
}

.font-weight-medium {
  font-weight: 500;
}

/* owl */
.owl-carousel .active span {
    width:10px;
    height:10px;
    margin:5px 7px;
    background: var(--primaryColor) !important;
    display:block;
    /* -webkit-backface-visibility:visible; */
    -webkit-transition:opacity 200ms ease;
    -moz-transition:opacity 200ms ease;
    -ms-transition:opacity 200ms ease;
    -o-transition:opacity 200ms ease;
    transition:opacity 200ms ease;
    -webkit-border-radius:30px;
    -moz-border-radius:30px;
    border-radius:30px;
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
