<template>
  <div class="bg-banner-flash-sales">
    <div class="container">
      <!-- align-items-center -->
      <div class="row justify-content-between">
        <!-- col-3 -->
        <div class="col-8 col-lg-3 pl-4 pb-5 mx-auto m-lg-0 ">
          <div class="my-bg-primary pt-5 pb-5 mb-5">
            <div class="text-center">
              <h3 class="font-play my-text-white fs-60 font-weight-bold">FLASH</h3>
              <h3 class="font-play my-text-white fs-60 font-weight-bold">SALE</h3>

              <h5 class="my-text-white mb-4">UP TO 50% OFF</h5>
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-6 pt-5 pb-5 align-self-end">
          <!-- justify-content-between -->
          <div class="d-flex justify-content-between mb-2">
            <div
              class="count-down-bg d-flex flex-column justify-content-center text-center align-items-center"
            >
              <h5 class="m-0 color-primary font-play fs-36 font-weight-bold mycounter">7</h5>
              <p class="m-0">Days</p>
            </div>
            <div
              class="count-down-bg d-flex flex-column justify-content-center text-center align-items-center"
            >
              <h5 class="m-0 color-primary font-play fs-36 font-weight-bold mycounter">23</h5>
              <p class="m-0">Hours</p>
            </div>
            <div
              class="count-down-bg d-flex flex-column justify-content-center text-center align-items-center"
            >
              <h5 class="m-0 color-primary font-play fs-36 font-weight-bold mycounter">46</h5>
              <p class="m-0">Minutes</p>
            </div>
            <!-- only large -->
            <div class="d-none d-lg-block">
              <div
                class="count-down-bg d-flex flex-column justify-content-center text-center align-items-center"
              >
                <h5 class="m-0 color-primary font-play fs-36 font-weight-bold mycounter">12</h5>
                <p class="m-0">Seconds</p>
              </div>
            </div>
            <!--  -->
          </div>
          <!-- button -->
          <div class="d-flex justify-content-center mt-3 mb-2">
            <button
              class="btn rounded-pill color-primary text-uppercase pl-4 pr-4 btn-shopnow"
            >Shop Now</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};

$(document).ready(function () {
  // jquery.counterup använder jquery.waypoints
  // räknar upp från x till det värde som sätts i taggen tex. <strong class="header-Statistics-text mycounter" >1430</strong>
  // hämtar värde från class eller id med jquery
  let mycounter1 = $(".mycounter");
  mycounter1.counterUp({
    delay: 100,
    time: 1000,
    offset: 100,
    beginAt: 0,
  });
});
</script>

<style scoped>
.bg-banner-flash-sales {
  background-color: #0e153d;
}

.count-down-bg {
  background: url("/images/RoundDotted.png") no-repeat center;
  width: 112px;
  height: 112px;
}

.btn-shopnow {
  background-color: #ffffff;
  /* color: var(--); */
  font-size: 18px;
  font-weight: 500;
}
</style>