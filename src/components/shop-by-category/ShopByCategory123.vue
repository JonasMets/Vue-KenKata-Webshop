<template>
  <div class="container mt-5">
    <div class="d-flex justify-content-center font-play">
      <h2 class="fs-36 font-weight-bolder">
        SHOP BY
        <span class="color-primary fs-36 font-weight-bolder">CATEGORY</span>
      </h2>
    </div>
    <div class="d-flex justify-content-center">
      <img src="@/assets/wave.png" alt class />
    </div>
    <!--  d-flex justify-content-center-->
    <div class="d-flex justify-content-center">
      <p>We always try to give you the best product within a fast and reliable way</p>
    </div>

    <!-- css grid -->
    <div class="row overflow-hidden">
      <div class="col-12">
        <div class="grid-container">
          <div class="item1">
            <div class="category-men d-flex align-items-end rounded">
              <a href="#" class>
                <div class="bg-category">Men</div>
              </a>
            </div>
          </div>
          <div class="item2">
            <div class="category-women d-flex align-items-end rounded">
              <a href="#">
                <div class="bg-category">Women</div>
              </a>
            </div>
          </div>
          <div class="item3">
            <div class="category-kids d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Kids</div>
              </a>
            </div>
          </div>
          <div class="item4">
            <div class="category-shoes d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Shoes</div>
              </a>
            </div>
          </div>
          <div class="item5">
            <div class="category-hats d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Hats</div>
              </a>
            </div>
          </div>
          <div class="item6">
            <div class="category-sunglasses d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Sunglasses</div>
              </a>
            </div>
          </div>
          <div class="item7">
            <div class="category-watches d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Watches</div>
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- css grid end-->
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bg-category {
  background-color: #0e153d;
  color: #20d3c2;
  border-radius: 0 5px 0 5px;
  padding: 5px;
}

.category-men {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-women {
  height: 214px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-kids {
  height: 438px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-shoes {
  height: 438px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-hats {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-sunglasses {
  height: 214px;
  width: 438px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

.category-watches {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  /* margin: 0.5rem; */
  padding: 0;
}

/* css grid */
/* .grid-layout {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  grid-gap: 10px;
  grid-auto-rows: minmax(180px, auto);
  grid-auto-flow: dense;
  padding: 10px;
} */

/* .grid-item {
  padding: 1rem;
  font-size: 14px;
  font-weight: bold;
  text-transform: uppercase;
  color: #929796;
  background-color: #333;
  border-radius: 5px;
  
} */

/* .span-2 {
  grid-column-end: span 2;
  grid-row-end: span 2;
} */

/* .span-3 {
  grid-column-end: span 3;
  grid-row-end: span 4;
} */

/* css grid 2 */
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto auto;
  grid-gap: 10px;
  /* background-color: #2196f3; */
  /* padding: 10px; */
}
.item1 {
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 1;
  grid-column-end: 3;
}
.item2 {
  grid-row-start: 1;
  grid-row-end: 2;
  grid-column-start: 3;
  grid-column-end: 7;
}
.item3 {
  grid-row-start: 1;
  grid-row-end: 4;
  grid-column-start: 7;
  grid-column-end: 12;
}
.item4 {
  grid-row-start: 2;
  grid-row-end: 5;
  grid-column-start: 1;
  grid-column-end: 5;
}

.item5 {
  grid-row-start: 2;
  grid-row-end: 4;
  grid-column-start: 5;
  grid-column-end: 7;
}
.item6 {
  grid-row-start: 4;
  grid-row-end: 5;
  grid-column-start: 5;
  grid-column-end: 9;
}
.item7 {
  grid-row-start: 4;
  grid-row-end: 5;
  grid-column-start: 9;
  grid-column-end: 12;
}

@media only screen and (max-width: 600px) {
  .grid-container {
  display: block;
  /* grid-template-columns: auto auto auto; */
  /* grid-gap: 10px; */
  /* background-color: #2196f3; */
  /* padding: 10px; */
}
}

</style>