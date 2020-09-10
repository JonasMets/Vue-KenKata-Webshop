<template>
  <div class="mybg-testimonials">
    <div class="text-center">
      <img src="@/assets/Quote.png" alt class="img-fluid" />
    </div>


      <div class="container mt-5">
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

            <div class="owl-carousel owl-theme" id="slider4">
              <!-- testimonial card slider-->
          <TestimonialsCard></TestimonialsCard>
          <TestimonialsCard></TestimonialsCard>
          <TestimonialsCard></TestimonialsCard>
          
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
import TestimonialsCard from "@/components/testimonials/TestimonialsCard.vue";

export default {

components:{
  TestimonialsCard
}

};


  $(document).ready(function () {
  // owl owl.carousel och owl.theme.default
  var owl4 = $("#slider4");
  owl4.owlCarousel({
    items: 2,
    dotsEach:true,
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
        items: 1,
        nav: false,
        loop: true,
      },
    },
  });

  // trigger next slide
  $(".customNextBtn").click(function () {
    owl4.trigger("next.owl.carousel");
  });
  // trigger next slide
  $(".customPrevBtn").click(function () {
    // With optional speed parameter
    // Parameters has to be in square bracket '[]'
    owl4.trigger("prev.owl.carousel", [300]);
  });
});


</script>

<style scoped>
.mybg-testimonials {
  background-color: var(--mydark-blue);
}


.btncls-1 {
  fill: none;
  stroke: #e3e3e3;
  stroke-linecap: round;
  stroke-miterlimit: 10;
  stroke-width: 2px;
}

.my-btn-prev-next {
  /* position: absolute; */
  /* top: 10px; */
  /* left: 10px; */
  background-color: var(--white);
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
  top: 160px;
  left: 50px;
  z-index: 2;
}

.my-btn-next-alignx {
  position: absolute;
  top: 160px;
  right: 10px;
  z-index: 2;
}


</style>