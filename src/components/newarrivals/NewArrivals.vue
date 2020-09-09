<template>
  <div>
    <div class="container mt-5 justify-content-center text-center">
      <div class="row">
        <div class="col">
          <div class="d-flex justify-content-center font-play">
            <h2 class="fs-36 font-weight-bolder">
              NEW
              <span class="color-primary fs-36 font-weight-bolder">ARRIVALS</span>
            </h2>
          </div>
          <div class="d-flex justify-content-center">
            <img src="@/assets/wave.png" alt class />
          </div>
          <!--  d-flex justify-content-center-->
          <div class="d-flex justify-content-center">
            <p>Check out our latest products from top fashion designers</p>
          </div>
        </div>
      </div>
    </div>

    <!-- här ska det vara en carousel med    cards? -->
    <!-- card -->
    <!-- <CardNewArrivals></CardNewArrivals> -->
    <div class="container justify-content-center">
      <div class="row justify-content-center align-items-center">
        <div class="col justify-content-center">
          <!-- :autoplay="true" :items="3" :loop="true" id="slider1" -->
          <!-- vue-owl -->
          <!-- <carousel
            :autoplay="true"
            :nav="false"
            :items="3"
            :loop="true"
            :dots="true"
            :responsive="{0:{items:1,nav:false},600:{items:2,nav:false},1100:{items:3,nav:false}}"
            :autoplayHoverPause="true"
          >
            <CardNewArrivals
              v-for="(product, index) in newProducts"
              :key="index"
              :product="product"
            />
          </carousel> -->

          <!--std Owl -->
          <div class="row align-items-center justify-content-center">
            <div class="col-7 col-md-12 col-lg-12">
              <div class="owl-carousel owl-theme" id="slider2">
                <!-- <div class="item d-flex justify-content-center align-items-center"> -->
                  <CardNewArrivals
                    v-for="(product, index) in newProducts"
                    :key="index"
                    :product="product"
                  />
                <!-- </div> -->
              </div>
            </div>
          </div>
          <!-- std Owl end -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardNewArrivals from "@/components/newarrivals/CardNewArrivals.vue";

import carousel from "vue-owl-carousel";

export default {
  components: {
    CardNewArrivals,
    carousel,
  },
  data() {
    return {
      newProducts: [
        {
          category: "Shirt",
          name: "Blue silk flare sleeved top",
          targetprice: "$25",
          price: "$19.00",
          badge: "NEW",
          image: require("@/assets/Productsleeve.png"),
        },
        {
          category: "Coat",
          name: "New look men's coat",
          targetprice: "$220",
          price: "$190.00",
          badge: "NEW",
          image: require("@/assets/MensCoat.png"),
        },
        {
          category: "Sport wear",
          name: "Circle pattern girls shirt",
          targetprice: "$120",
          price: "$99",
          badge: "NEW",
          image: require("@/assets/GirlsShirt.png"),
        },
        {
          category: "Outwear",
          name: "Black jacket",
          targetprice: "$200",
          price: "$150",
          badge: "NEW",
          image: require("@/assets/MensCoat.png"),
        },
      ],
    };
  },
};


$(document).ready(function () {
  // owl owl.carousel och owl.theme.default
  var owl2 = $("#slider2");
  owl2.owlCarousel({
    items: 4,
    loop: true,
    margin: 10,
    autoplay: true,
    autoplayTimeout: 3000,
    autoplayHoverPause: true,
    // ändrar antal som ska visas responsivt
    responsive: {
      0: {
        items: 1,
        nav: false,
      },
      600: {
        items: 1,
        nav: false,
        loop: true,
      },
      1000: {
        items: 3,
        nav: false,
        loop: true,
      },
    },
  });
});

</script>

<style >
</style>