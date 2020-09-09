<template>
  <div class="bg-banner1">
    <div class="container">
      <div class="row justify-content-center align-items-center">
        <!-- -12 col-md-4 col-lg-6 -->
        <div class="col justify-content-center align-items-center">
          <div>
            <div class="my-bg-primary full-height text-center width-255 pt-5 pb-5">
              <h3 class="font-play my-text-white fs-60 font-weight-bold mt-5 mb-1">
                30%
                <span class="font-play my-text-white fs-36 font-weight-bold">off</span>
              </h3>
              <h5 class="my-text-white mb-4">for new customer</h5>
              <button class="btn rounded-pill btn-shop-now pl-4 pr-4 mb-5">Shop Now</button>
            </div>
          </div>
        </div>

<!-- -12 col-md-4 col-lg-6 -->
        <div class="col">
          <p class="my-text-white">Donec pulvinar arcu vitae ipsum varius cursus. Nunc iaculis fermentum iaculis. Nunc pulvinar purus at erat lacinia, ut convallis nibh consequat. Integer nulla nisi, aliquam at tellus a, viverra scelerisque purus. Nam pretium iaculis ultrices.</p>
          <button class="btn rounded-pill btn-learn-now pl-4 pr-4 mb-5">LEARN MORE</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-banner1 {
  background-color: #CCCCCC;
}

.full-height {
  height: 100%;
}

.width-255 {
  width: 255px;
}

.btn-shop-now {
  background-color: var(--mydark-blue);
  color: var(--white);
}

.btn-learn-now {
  background-color: #ffffff;
  color: var(--primaryColor);
  font-size: 18px;
  font-weight: 500;
}
</style>