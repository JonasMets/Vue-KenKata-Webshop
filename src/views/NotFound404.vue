<template>
  <div class="bg-not-found">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-6 mt-5">
          <img src="images/404.png" alt class="img-fluid" />
        </div>
      </div>
      <div class="row justify-content-center ">
        <div class="col-6 mb-5 mt-5">
          <!--  -->
          <div class="text-center">
            <p class="fs-24 font-weight-medium">Oops! The page you are looking for doesn't exist.</p>
          </div>
          <!--  -->
          <div class="d-flex justify-content-center">
            <button
              class="btn rounded-pill color-primary my-bg-primary btn-outline-secondary text-light border-0 pl-4 pr-4"
              type="button"><router-link to="/home" class="text-light">HOME</router-link></button>
            <button class="btn rounded-pill my-bg-dark-blue text-light ml-4 pl-4 pr-4">CONTACT US</button>
          </div>

          <!--  -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-not-found {
  background-color: #f6f6f6;
}
</style>