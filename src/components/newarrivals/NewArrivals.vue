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




  </div>
</template>

<script>
import CardNewArrivals from "@/components/newarrivals/CardNewArrivals.vue";

export default {

components :{
  CardNewArrivals 
}

};
</script>

<style scoped>

</style>