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
    <CardNewArrivals></CardNewArrivals>

<!-- test -->
    <!-- <div class="container">
      <button
        type="button"
        class="btn btn-secondary"
        data-toggle="tooltip"
        data-placement="left"
        title="Tooltip on left"
      >Tooltip on left</button>
    </div> -->


  </div>
</template>

<script>
import CardNewArrivals from "@/components/newarrivals/CardNewArrivals.vue";

export default {
  components: {
    CardNewArrivals,
  },
};
</script>

<style >

/* .tooltip > .tooltip-inner {
  background-color: red;
} */

/* .tooltip.bs-tooltip-auto[x-placement^="left"] .arrow::before,
.tooltip.bs-tooltip-left .arrow::before {
  border-left-color: red;
} */

</style>