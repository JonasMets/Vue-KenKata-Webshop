<template>
  <!--          container -->
  <div class="overflow-hidden mt-5">

    <div class="row align-items-center justify-content-center">
      <div class="col-7 col-md-12 col-lg-12">
        <div class="owl-carousel owl-theme" id="slider1">
          <div class="item d-flex justify-content-center align-items-center">
            <div id="arguments1" class="d-flex align-items-center rounded">
              <svg class="icons">
                <use xlink:href="@/assets/24icon.svg#_24_icon" />
              </svg>
              <div class="argument-text">
                <p class="color-primary">24/7 Support</p>
                <p>For any inquiry, we are available 24 hours every day</p>
              </div>
            </div>
          </div>
          <div class="item d-flex justify-content-center align-items-center ">
            <div id="arguments1" class="d-flex align-items-center rounded">
              <svg class="icons">
                <use xlink:href="@/assets/freeshipping.svg#Path_593" />
              </svg>
              <div class="argument-text">
                <p class="color-primary">Free Shipping</p>
                <p>For a local customer, we provide free shipping facility</p>
              </div>
            </div>
          </div>
          <div class="item d-flex justify-content-center align-items-center ">
            <div id="arguments1" class="d-flex align-items-center rounded">
              <svg class="icons">
                <use xlink:href="@/assets/onlinepayment.svg#Path_36" />
              </svg>
              <div class="argument-text">
                <p class="color-primary">Online payment</p>
                <p>You can pay quickly and easily with our online payment system</p>
              </div>
            </div>
          </div>
          <div class="item d-flex justify-content-center align-items-center ">
            <div id="arguments1" class="d-flex align-items-center rounded">
              <svg class="icons">
                <use xlink:href="@/assets/Group1158.svg#Group_1158" />
              </svg>
              <div class="argument-text">
                <p class="color-primary">Fast delivery</p>
                <p>We understand your urgency and we deliver in a fast way</p>
              </div>
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
#arguments1 {
  background-color: rgba(32, 211, 194, 0.1);
  /* padding-top: 20px; */
  width: 397px;
  min-height: 137px;
}
#arguments1:hover {
  background-color: rgba(32, 211, 194, 1);
  color: #fff;
}

#arguments1:hover p{
  color: #fff;
}

#arguments1:hover .icons{
  fill: #fff;
}

/* #20d3c2 */
.icons {
  width: 80px;
  height: 55px;
  margin-left: 25px;
  margin-right: 20px;
  fill: #20d3c2;
}

.argument-text {
  margin-right: 35px;
}

</style>