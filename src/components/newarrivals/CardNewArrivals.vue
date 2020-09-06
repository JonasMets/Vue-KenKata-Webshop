<template>
  <div>
    <!-- d-flex justify-content-center -->
    <div class="container">
      <!-- style="width: 18rem;" -->
      <div class="card text-center position-relative" style="width: 18rem;">
        <div>
          <!--  rounded-circle d-flex justify-content-center-->
          <div class=" myAlert1 d-flex align-items-center justify-content-center">New</div>
          <img src="@/assets/Productsleeve.png" class="card-img-top my-img-bg img-fluid" alt="sleeve" />
        </div>
        <div class="card-footer myCard-footer text-left">Blue silk flare sleeved top</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>

  .myCard-footer {
    background-color: var(--mydark-blue);
    color: var(--white);
    font-size: 18px;
  }

  .myAlert1 {
    position: absolute;
    top: 10px;
    left: 10px;
    background-color: var(--primaryColor);
    color: var(--white);
    /* padding: 5px; */
    height: 60px;
    width: 60px;
    border-radius: 50%;
  }

  .my-img-bg {
    background-color: #eeeeee;
  }


</style>