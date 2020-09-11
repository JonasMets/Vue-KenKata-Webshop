<template>
  <!-- d-flex -->
  <div class>
    <div class="card blog-card posistion-relative">
      <!--  -->
      <div class="card blog-card-info-bg d-flex flex-column justify-content-center">
        <div
          class="blog-card-info-date d-flex flex-column align-items-center justify-content-center"
        >
          <p class="p-0 m-0 font-play my-text-white fs-36">{{blog.date}}</p>
          <p class="p-0 m-0 my-text-white"> {{blog.month}} </p>
        </div>

        <div class="ml-4 mt-5 pt-2">
          <!-- d-flex align-items-center -->
          <div class="d-block">
            <div class="my-text-white fz-14">
              By 
              <a class=" my-text-white fz-14 " href="#">{{blog.name}}</a> 
            </div>
          </div>

          <div class>
            <p class="color-primary text-wrap fs-16 font-weight-medium overflow-hidden" style="width: 12rem;">
              {{blog.blogText}}
            </p>
          </div>
          <!--  -->
          <div class="d-flex justify-content-between" style="width: 8.5rem;">
            <button type="button" class="btn btn-sm text-light my-btn-border">Travel</button>
            <button type="button" class="btn btn-sm text-light my-btn-border">Fashion</button>
          </div>
          <div>
            <button
              class="btn rounded-pill color-primary btn-readmore fs-16 pl-3 pr-3 mt-3"
            >Read Moore</button>
          </div>

          <!--  -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

props: {
    blog: {},
  }

};
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

.my-btn-border {
  border-color: var(--white) !important;
}

.btn-readmore {
  background-color: #ffffff;
  /* color: var(--); */
  font-size: 18px;
  font-weight: 500;
}
</style>