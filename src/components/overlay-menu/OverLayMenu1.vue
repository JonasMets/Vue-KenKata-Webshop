<template>
  <!-- OverLayMenu1  -->
  <div id="overlaysidemenu1" class="overlay-side-menu rounded-pill pt-3 pb-3">
    <!-- round circle for color select-->
    <div class="my-color-selector" data-toggle="tooltip" data-placement="left" title="Select Color"></div>

    <a href="#" class data-toggle="tooltip" data-placement="left" title="Like/Add To Favourites">
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Hearticon.svg#Heart_icon" class />
      </svg>
    </a>

    <a href="#" data-toggle="tooltip" data-placement="left" title="Compare Items">
      <!--  -->
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Compareicon.svg#Compare_icon" class />
      </svg>
    </a>
    <a href="#" data-toggle="tooltip" data-placement="left" title="Search Item">
      <!--  -->
      <svg class="icons cls-1">
        <use xlink:href="@/assets/Searchicon.svg#Search_icon" class />
      </svg>
    </a>
    <a href="#" class="tooltipChange" data-toggle="tooltip" data-placement="left" title="Add To Cart">
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
  $('[data-toggle="tooltip"]').tooltip();
  // $("a").tooltip();
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
  background-color: #20d3c2 ;
  opacity: 1;
}

.tooltip.bs-tooltip-auto[x-placement^="left"] .arrow::before,
.tooltip.bs-tooltip-left .arrow::before {
  border-left-color: #20d3c2 ;
  opacity: 1;
}

</style>