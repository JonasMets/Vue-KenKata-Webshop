<template>
  <div>
    <!-- overhead text -->
    <div class="container mt-5 justify-content-center text-center">
      <div class="row">
        <div class="col">
          <div class="d-flex justify-content-center font-play">
            <h2 class="fs-36 font-weight-bolder">
              LATEST
              <span class="color-primary fs-36 font-weight-bolder">BLOG</span>
            </h2>
          </div>
          <div class="d-flex justify-content-center">
            <img src="@/assets/wave.png" alt class />
          </div>
          <!-- -->
          <div class="d-flex justify-content-center">
            <p>Read our latest posts about our events and trending news</p>
          </div>
        </div>
      </div>
    </div>

    <div class="container">
      <!--  -->
      <LatestBlogCard></LatestBlogCard>
    </div>

  </div>
</template>

<script>

import LatestBlogCard from "@/components/latest-blog/LatestBlogCard.vue";

export default {
  components:{
    LatestBlogCard
  }

};
</script>

<style>
</style>