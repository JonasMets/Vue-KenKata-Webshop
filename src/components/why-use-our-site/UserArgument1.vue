<template>
  <!--          container -->
  <div class="overflow-hidden">
    <h3>why use us argument here</h3>

    <!-- #_24_icon -->
    <!-- <svg class="logo">
      <use xlink:href="@/assets/24icon.svg#_24_icon" />
    </svg>-->

    <div class="row align-items-center justify-content-center">
      <div class="col-7 col-md-12 col-lg-12">
        <div class="owl-carousel owl-theme" id="slider1">
          <div class="item d-flex justify-content-center align-items-center bg-arguments">
            <svg class="icon24-7">
              <use xlink:href="@/assets/24icon.svg#_24_icon" />
            </svg>
            <div>
              <p class="color-primary">Free Shipping</p>
              <p>For a local customer, we provide free shipping facility</p>
            </div>
          </div>
          <div class="item d-flex justify-content-center align-items-center bg-arguments">
            <svg class="icon24-7">
              <use xlink:href="@/assets/24icon.svg#_24_icon" />
            </svg>
            <div>
              <p class="color-primary">Free Shipping</p>
              <p>For a local customer, we provide free shipping facility</p>
            </div>
          </div>
          <div class="item d-flex justify-content-center align-items-center bg-arguments">
            <svg class="icon24-7">
              <use xlink:href="@/assets/24icon.svg#_24_icon" />
            </svg>
            <div>
              <p class="color-primary">Free Shipping</p>
              <p>For a local customer, we provide free shipping facility</p>
            </div>
          </div>
          <div class="item d-flex justify-content-center align-items-center bg-arguments">
            <svg class="icon24-7">
              <use xlink:href="@/assets/24icon.svg#_24_icon" />
            </svg>
            <div>
              <p class="color-primary">Free Shipping</p>
              <p>For a local customer, we provide free shipping facility</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};

$(document).ready(function () {
  // owl owl.carousel och owl.theme.default
  var owl = $("#slider1");
  owl.owlCarousel({
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
        nav: true,
      },
      600: {
        items: 3,
        nav: true,
        loop: true,
      },
      1000: {
        items: 4,
        nav: true,
        loop: true,
      },
    },
  });
});
</script>

<style scoped>

.bg-arguments {
  /* background: rgb(32, 211, 194) ; */
  background-color: rgba(32, 211, 194, 0.2);
  /* opacity: 0.1; */
}
.bg-arguments:hover {
  /* background: rgb(32, 211, 194) ; */
  background-color: rgba(32, 211, 194, 1);
  /* opacity: 0.1; */
  color: #fff;
}

/* #20d3c2 */
.icon24-7 {
  width: 80px;
  height: 50px;
  margin-left: 5px;
  margin-right: 20px;
  fill: #20d3c2;
}
/* .icon24-7:hover {
  fill: #fff;
} */
</style>