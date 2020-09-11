<template>
  <div class="bg-banner-subscribe">
    <div class="container">
      <div class="row align-items-center justify-content-between">
        <div class="col-12 col-lg-5">
          <!-- d-flex justify-content-center -->
          <div class="font-play">
            <h2 class="fs-36 font-weight-bolder text-uppercase">
              Subscribe
              <span class="color-primary fs-36 font-weight-bolder">Now</span>
            </h2>
          </div>
          <!-- d-flex justify-content-center -->
          <div class>
            <p class="text-wrap" style="width: 26rem;">
              Signup for awesome news about our new products and
              know our special discounts on products.
            </p>
          </div>
          <div class="my-input-area rounded-pill border">
            <div class="input-group border-0">
              <input
                type="text "
                class="form-control border-0 ml-2"
                placeholder="Enter email address"
                aria-label="Enter email address"
                aria-describedby="button-addon2"
              />
              <div class="input-group-append">
                <!-- btn-outline-secondary -->
                <button
                  class="btn rounded-pill color-primary my-bg-primary btn-outline-secondary text-light"
                  type="button"
                  id="button-addon2"
                >Subscribe</button>
              </div>
            </div>
          </div>
        </div>
        <!-- col end -->
        <div class="col-lg-6 d-none d-lg-block">
          <img src="@/assets/Backgroundimage.png" alt="" class="img-fluid">
        </div>
        <!-- col end -->
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-banner-subscribe {
  background-color: #f6f6f6;
}

.my-input-area{
  background-color: #fff;
  padding: 2px 5px 2px 5px;
}

</style>