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

    <!-- <div class="container">
      <LatestBlogCard></LatestBlogCard>
    </div>-->

    <!-- row -->
    <div class="container">
      <!--   overflow-hidden -->
      <div class="row align-items-center justify-content-center position-relative">
        <!-- button prev -->
        <div class="col-1 d-none d-xl-block m-0 p-0 my-btn-prev-alignx">
          <button class="btn my-btn-prev-next customPrevBtn">
            <i class="fas fa-chevron-left fa-2x"></i>
          </button>
        </div>

        <div class="col-12">
          <!--        container -->
          <div class="justify-content-center">
            <!--std Owl -->

            <div class="owl-carousel owl-theme" id="slider5">
              <!---->

              <LatestBlogCard
                v-for="(blog, index) in latestBlogs"
                :key="index"
                :blog="blog"
              />
            </div>
          </div>
        </div>
        <!-- carousel section end -->

        <!-- button next align-self-center d-flex justify-content-start-->
        <div class="col-1 d-none d-xl-block m-0 p-0 my-btn-next-alignx">
          <button class="btn my-btn-prev-next customNextBtn">
            <i class="fas fa-chevron-right fa-2x"></i>
          </button>
        </div>
      </div>
      <!-- row end -->
    </div>
  </div>
</template>

<script>
import LatestBlogCard from "@/components/latest-blog/LatestBlogCard.vue";

export default {
  components: {
    LatestBlogCard,
  },
  data() {
    return {
      latestBlogs: [
        {
          category: "Blog",
          date:29,
          month:"MAR",
          name: "Adam Moore",
          blogText: "A beautiful scenery in the world we are missing",
          tags: ["Travel", "Fashion"],
        },
        {
          category: "Blog",
          date:18,
          month:"JUL",
          name: "Jonathon Doe",
          blogText: "We love our country, we love our peoples like ourselves",
          tags: ["Travel", "Fashion"],
        },
        {
          category: "Blog",
          date:2,
          month:"MAR",
          name: "Adam Foore",
          blogText: "A beautiful scenery we are missing in the world we are",
          tags: ["Travel", "Fashion"],
        },
      ],
    };
  },
};

$(document).ready(function () {
  // owl owl.carousel och owl.theme.default
  var owl5 = $("#slider5");
  owl5.owlCarousel({
    items: 3,
    dotsEach: true,
    loop: true,
    margin: 10,
    autoplay: true,
    autoplayTimeout: 3000,
    autoplayHoverPause: true,
    autoplaySpeed: 1500,
    // ändrar antal som ska visas responsivt
    responsive: {
      0: {
        items: 1,
        nav: false,
      },
      600: {
        items: 1,
        nav: false,
        loop: true,
      },
      1000: {
        items: 2,
        nav: false,
        loop: true,
      },
    },
  });

  // trigger next slide
  $(".customNextBtn").click(function () {
    owl5.trigger("next.owl.carousel");
  });
  // trigger next slide
  $(".customPrevBtn").click(function () {
    // With optional speed parameter
    // Parameters has to be in square bracket '[]'
    owl5.trigger("prev.owl.carousel", [300]);
  });
});
</script>

<style scoped>
.my-btn-prev-next {
  /* position: absolute; */
  /* top: 10px; */
  /* left: 10px; */
  /* background-color: var(--primaryColor); */
  color: #e3e3e3;
  /* padding: 5px; */
  height: 60px;
  width: 60px;
  border-radius: 50%;
  border-color: #e3e3e3;
}

.my-btn-prev-next:hover {
  background-color: var(--primaryColor);
  border-color: #e3e3e3;
}

.my-btn-prev-alignx {
  position: absolute;
  top: 180px;
  left: -50px;
  z-index: 2;
}

.my-btn-next-alignx {
  position: absolute;
  top: 180px;
  right: -90px;
  z-index: 2;
}
</style>