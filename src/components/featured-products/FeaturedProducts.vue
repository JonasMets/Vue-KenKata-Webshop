<template>
  <div>
    <!-- overhead text -->
    <div class="container mt-5 justify-content-center text-center">
      <div class="row">
        <div class="col">
          <div class="d-flex justify-content-center font-play">
            <h2 class="fs-36 font-weight-bolder">
              FEATURED
              <span class="color-primary fs-36 font-weight-bolder">PRODUCTS</span>
            </h2>
          </div>
          <div class="d-flex justify-content-center">
            <img src="@/assets/wave.png" alt class />
          </div>
          <!-- -->
          <div class="d-flex justify-content-center">
            <p>Check out our monthly featured products from top brands</p>
          </div>
        </div>
      </div>
    </div>

    <!-- row -->
    <div class="container">
      <!--   overflow-hidden -->
      <div class="row align-items-center justify-content-center position-relative">
        <!-- button prev -->
        <div class="col-1 d-none d-xl-block m-0 p-0 my-btn-prev-alignx">
          <button class="btn my-btn-prev-next customPrevBtn">
            <i class="fas fa-chevron-left fa-2x"></i>
          </button>
        </div>

        <div class="col-12">
          <!--        container -->
          <div class="justify-content-center">
            <!--std Owl -->

            <div class="owl-carousel owl-theme" id="slider3">
              <!-- class="item d-flex justify-content-center align-items-center" -->
              <CardFeaturedProducts
                v-for="(product, index) in newProducts"
                :key="index"
                :product="product"
              />
            </div>
          </div>
        </div>
        <!-- carousel section end -->

        <!-- button next align-self-center d-flex justify-content-start-->
        <div class="col-1 d-none d-xl-block m-0 p-0 my-btn-next-alignx">
          <button class="btn my-btn-prev-next customNextBtn">
            <i class="fas fa-chevron-right fa-2x"></i>
          </button>
        </div>
      </div>
      <!-- row end -->
    </div>
    <!-- container end -->
  </div>
  <!-- end div -->
</template>

<script>
import CardFeaturedProducts from "@/components/featured-products/CardFeaturedProducts.vue";

import carousel from "vue-owl-carousel";

export default {
  components: {
    CardFeaturedProducts,
    carousel,
  },
  data() {
    return {
      newProducts: [
        {
          category: "Outwear",
          name: "Winter collection for women's",
          targetprice: "$25",
          price: "$19.00",
          badge: "HOT",
          image: require("@/assets/Productsleeve.png"),
          rating:5
        },
        {
          category: "Coat",
          name: "New look men's coat",
          targetprice: "$220",
          price: "$190.00",
          badge: "NEW",
          image: require("@/assets/MensCoat.png"),
          rating:5
        },
        {
          category: "Outwear",
          name: "Red women's blazer full",
          targetprice: "$120",
          price: "$99",
          badge: "-30%",
          image: require("@/assets/GirlsShirt.png"),
          rating:5
        },
        {
          category: "Outwear",
          name: "Black jacket",
          targetprice: "$200",
          price: "$150",
          badge: "NEW",
          image: require("@/assets/MensCoat.png"),
          rating:5
        },
      ],
    };
  },
};

$(document).ready(function () {
  // owl owl.carousel och owl.theme.default
  var owl3 = $("#slider3");
  owl3.owlCarousel({
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

  // trigger next slide
  $(".customNextBtn").click(function () {
    owl3.trigger("next.owl.carousel");
  });
  // trigger next slide
  $(".customPrevBtn").click(function () {
    // With optional speed parameter
    // Parameters has to be in square bracket '[]'
    owl3.trigger("prev.owl.carousel", [300]);
  });
});
</script>

<style scoped>
.btncls-1 {
  fill: none;
  stroke: #e3e3e3;
  stroke-linecap: round;
  stroke-miterlimit: 10;
  stroke-width: 2px;
}

.my-btn-prev-next {
  /* position: absolute; */
  /* top: 10px; */
  /* left: 10px; */
  /* background-color: var(--primaryColor); */
  color: #e3e3e3;
  /* padding: 5px; */
  height: 60px;
  width: 60px;
  border-radius: 50%;
  border-color: #e3e3e3;
}

.my-btn-prev-next:hover {
  background-color: var(--primaryColor);
  border-color: #e3e3e3;
}

.my-btn-prev-alignx {
  position: absolute;
  top: 180px;
  left: -50px;
  z-index: 2;
}

.my-btn-next-alignx {
  position: absolute;
  top: 180px;
  right: -90px;
  z-index: 2;
}
</style>