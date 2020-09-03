<template>
  <div class="bg-banner1">
    <div class="container">
      <!-- <h2>Banner carousel here</h2> -->
      <!--                                                                           data-interval="5000"-->
      <div id="carouselExampleSlidesOnly" class="carousel slide" data-ride="carousel" data-interval="6000">
        <div class="carousel-inner">
          <div class="carousel-item active">
            <div class="row align-items-center">
              <div class="col">
                <div>
                  <h2 class="font-play fs-60">Shopping is</h2>
                  <h2 class="font-play font-weight-bold fs-60 color-primary">MORE FUN</h2>
                </div>
                <div>
                  <p
                    class
                  >Vivamus dignissim a ex eu ornare. Ut fermentum orci vel diam ultricies faucibus. Quisque quis erat sed</p>
                </div>

                <button
                  class="btn rounded-pill color-primary text-uppercase pl-4 pr-4 btn-shopnow"
                >Shop Now</button>
              </div>
              <div class="col">
                <img src="@/assets/Banner-thumb.png" class="d-block w-100" />
              </div>
            </div>
          </div>
          <div class="carousel-item">
            <div class="row align-items-center">
              <div class="col">
                <div>
                  <h2 class="font-play">MORE FUN</h2>
                  <h2 class="font-play font-weight-bold fs-60 color-primary text-uppercase">Shopping is</h2>
                </div>
                <div>
                  <p
                    class
                  >Vivamus dignissim a ex eu ornare. Ut fermentum orci vel diam ultricies faucibus. Quisque quis erat sed</p>
                </div>

                <button
                  class="btn rounded-pill color-primary text-uppercase pl-4 pr-4 btn-shopnow"
                >Shop Now</button>
              </div>
              <div class="col">
                <img src="@/assets/Banner-thumb.png" class="d-block w-100" />
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
</script>

<style scoped>
.bg-banner1 {
  background-color: #eeeeee;
}

.myfont-bold {
  font-weight: 900 !important;
}
.fs-60 {
  font-size: 60px;
}

.btn-shopnow {
  background-color: #ffffff;
  /* color: var(--); */
  font-size: 18px;
  font-weight: 500;
}
</style>