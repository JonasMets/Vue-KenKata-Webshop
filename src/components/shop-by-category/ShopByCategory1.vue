<template>
  <div class="container mt-5">
    <div class="d-flex justify-content-center font-play">
      <h2 class="fs-36 font-weight-bolder">
        SHOP BY
        <span class="color-primary fs-36 font-weight-bolder">CATEGORY</span>
      </h2>
    </div>
    <div class="d-flex justify-content-center">
      <img src="@/assets/wave.png" alt class />
    </div>
    <!--  d-flex justify-content-center-->
    <div class="d-flex justify-content-center">
      <p>We always try to give you the best product within a fast and reliable way</p>
    </div>

    <!-- categories -->
    <!-- 7 items -->
    <div class="container">
      <div class="row justify-content-around ">
        <div class="col category-men d-flex align-items-end rounded">
          <div class="bg-category">Men</div>
        </div>
        <div class="col category-women d-flex align-items-end rounded">
          <div class="bg-category">Women</div>
        </div>
        <div class="col category-kids d-flex align-items-end rounded">
          <div class="bg-category">Kids</div>
        </div>
        <div class="col category-shoes d-flex align-items-end rounded">
          <div class="bg-category">Shoes</div>
        </div>
        <div class="col category-hats d-flex align-items-end rounded">
          <div class="bg-category">Hats</div>
        </div>
        <div class="col category-sunglasses d-flex align-items-end rounded">
          <div class="bg-category">Sunglasses</div>
        </div>
        <div class="col category-watches d-flex align-items-end rounded">
          <div class="bg-category">Watches</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-category {
  background-color: #0e153d;
  color: #20d3c2;
  border-radius: 0 5px 0 5px;
  padding: 5px;
}

.category-men {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-women {
  height: 214px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-kids {
  height: 438px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-shoes {
  height: 438px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-hats {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-sunglasses {
  height: 214px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-watches {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}
</style>