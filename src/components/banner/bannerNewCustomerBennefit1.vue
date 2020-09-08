<template>
  <div class="bg-banner1">
    <div class="container">
      <div class="row">
        <div class="col-12 col-md-4 col-lg-6">
          <div class="my-bg-primary full-height">
            <h3>30% off</h3>
            <h5>for new customer</h5>
            <button class="btn rounded-pill btn-shop-now">Shop Now</button>
          </div>
        </div>
        <div class="col-12 col-md-4 col-lg-6">
          <p>Donec pulvinar arcu vitae ipsum varius cursus. Nunc iaculis fermentum iaculis. Nunc pulvinar purus at erat lacinia, ut convallis nibh consequat. Integer nulla nisi, aliquam at tellus a, viverra scelerisque purus. Nam pretium iaculis ultrices.</p>
          <button class="btn rounded-pill btn-learn-now">Shop Now</button>
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
  background-color: #eeeeee;
}

.full-height {
  height: 100%;
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