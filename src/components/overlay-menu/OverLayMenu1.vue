<template>
  <!-- OverLayMenu1  -->
  <div id="overlaysidemenu1" class="overlay-side-menu rounded-pill pt-3 pb-3">
    
    <a href="" id="mytooltipcolorselector"
      class="my-color-selector" role="button" data-placement="left" 
      data-toggle="popover"></a>
    
    <a
      href="#"
      class="mytooltip1"
      data-toggle="tooltip"
      data-placement="left"
      title="Like/Add To Favourites"
    >
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Hearticon.svg#Heart_icon" class />
      </svg>
    </a>

    <a
      href="#"
      class="mytooltip1"
      data-toggle="tooltip"
      data-placement="left"
      title="Compare Items"
    >
      <!--  -->
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Compareicon.svg#Compare_icon" class />
      </svg>
    </a>
    <a href="#" class="mytooltip1" data-toggle="tooltip" data-placement="left" title="Quick view">
      <!--  -->
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Searchicon.svg#Search_icon" class />
      </svg>
    </a>
    <a href="#" class="mytooltip1" data-toggle="tooltip" data-placement="left" title="Add To Cart">
      <!-- -->
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Cart2.svg#Cart2" class />
      </svg>
    </a>

  </div>
</template>

<script>
export default {};

$(document).ready(function () {

let colors = '<div class="d-flex">  <div class="my-color-dot-black mr-1 ml-1 order-4"> </div> <div class="my-color-dot-pink mr-1 ml-1 order-3"> </div> <div class="my-color-dot-purple mr-1 ml-1 order-2"> </div> <div class="my-color-dot-turquoise mr-1 ml-1 order-1"> </div>  </div>';

let images ='<img src="http://placehold.it/20x20" alt="" class="my-color-dot-black"> <img src="http://placehold.it/20x20" alt="" class="my-color-dot-black"> <img src="http://placehold.it/20x20" alt="" class="my-color-dot-black"> <img src="http://placehold.it/20x20" alt="" class="my-color-dot-black">';

let images2 = '<img src="images/TurquoiseDot.png" alt=""> <img src="images/PurpleDot.png" alt="">  <img src="images/PinkDot.png" alt=""> <img src="images/BlackDot.png" alt="">';
// let images2 = '<img src="@/assets/BlackDot.png" alt="">  ';

  // 
  $(".mytooltip1").tooltip();

$('[data-toggle="popover"]').popover({
   trigger: "manual",
    html: true ,
    // return ' <img src="http://placehold.it/20x20" alt="" class="my-color-selector">'
    content: function () { return images2; }, 
   animation:false
   })
    .on("mouseenter", function () {
        var _this = this;
        $(this).popover("show");
        $(".popover").on("mouseleave", function () {
            $(_this).popover('hide');
        });
    }).on("mouseleave", function () {
        var _this = this;
        setTimeout(function () {
            if (!$(".popover:hover").length) {
                $(_this).popover("hide");
            }
        }, 300);
});


});
</script>

<style >
.overlay-side-menu {
  display: flex;
  flex-flow: column;
  background-color: var(--white);
  width: 46px;
  height: 203px;
  justify-content: space-between;
  align-items: center;
}

.my-color-selector {
  background-color: #fe6c6c;
  width: 20px;
  height: 20px;
  border-radius: 50%;
}

.my-color-dot-black {
  background-color: #333333;
  color: #333333;
  width: 13px;
  height: 13px;
  border-radius: 50%;
}
.my-color-dot-pink {
  background-color: #FE6C6C;
  width: 13px;
  height: 13px;
  border-radius: 50%;
}
.my-color-dot-purple {
  background-color: #CA82D8;
  width: 13px;
  height: 13px;
  border-radius: 50%;
}
.my-color-dot-turquoise {
  background-color: #82D8C6;
  width: 13px;
  height: 13px;
  border-radius: 50%;
}

#overlaysidemenu1 .icons {
  width: 22px;
  height: 21px;
}

a .cls-1 {
  fill: none;
  stroke: #aaa;
  stroke-linecap: round;
  stroke-linejoin: round;
  stroke-width: 1.5px;
}
a .cls-1:hover {
  fill: none;
  stroke: #20d3c2;
  stroke-linecap: round;
  stroke-linejoin: round;
  stroke-width: 1.5px;
}

#overlaysidemenu1 a:hover {
  stroke: #20d3c2 !important;
}

/* tooltip */
.tooltip > .tooltip-inner {
  background-color: #20d3c2;
  opacity: 1;
}

.tooltip.bs-tooltip-auto[x-placement^="left"] .arrow::before,
.tooltip.bs-tooltip-left .arrow::before {
  border-left-color: #20d3c2;
  opacity: 1;
}

/* my popper  */
.popover{
    max-width: 200px; /* Max Width of the popover (depending on the container!) */
}
</style>