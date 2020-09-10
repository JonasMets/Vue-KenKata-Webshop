<template>
  <div class="d-flex">
    <div class="card blog-card posistion-relative">
      <!--  -->
      <div class="card blog-card-info-bg d-flex flex-column justify-content-center">
        <div
          class="blog-card-info-date d-flex flex-column align-items-center justify-content-center"
        >
          <p class="p-0 m-0 font-play my-text-white fs-36">29</p>
          <p class="p-0 m-0 my-text-white">MAR</p>
        </div>

        <div class="ml-4">
          <p class="my-text-white fz-14">
            By
            <span>
              <a href class="my-text-white">Adam Moore</a>
            </span>
          </p>
          <div class="">
            <p class="color-primary text-wrap fs-16 font-weight-medium" style="width: 12rem;">
              A beautiful scenery in the
              world we are missing
            </p>
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
.blog-card {
  height: 400px;
  width: 350px;
  background-color: #cccccc;
  padding: 0;
}

.blog-card-info-bg {
  position: absolute;
  left: 250px;
  top: 48px;
  height: 304px;
  width: 275px;
  background-color: var(--mydark-blue);
  padding: 0;
}
.blog-card-info-date {
  position: absolute;
  left: 20px;
  top: 0;
  height: 77px;
  width: 60px;
  background-color: var(--primaryColor);
  padding: 0;
}
</style>