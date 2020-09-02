<template>
  <div class="bg-banner1">
    <div class="container">
      <!-- <h2>Banner carousel here</h2> -->

      <div class="row align-items-center">
        <div class="col">
          <div>
            <h2 class="font-play">Shopping is</h2>
            <h2 class="font-play font-weight-bold color-primary">MORE FUN</h2>
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
</template>

<script>
export default {};
</script>

<style scoped>
.bg-banner1 {
  background-color: #eeeeee;
}

.btn-shopnow {
  background-color: #ffffff;
  /* color: var(--); */
  font-size: 18px;
  font-weight: 500;
}
</style>