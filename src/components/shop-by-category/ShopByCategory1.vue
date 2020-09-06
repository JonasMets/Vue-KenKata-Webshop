<template>
  <div class="container mt-5 justify-content-center text-center">
    <div class="row">
      <div class="col">
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
      </div>
    </div>

    <!-- css grid -->
    <!-- <div class="row  overflow-hidden"> -->
      <!-- <div class="col"> -->
        <div class="grid-container justify-content-center">
          <div class="item1">

            <a href="#"> <div class="category-men category-d-sm d-flex align-items-end rounded">
              <a href="#" class>
                <div class="bg-category">Men</div>
              </a>
            </div>
            </a>

          </div>
          <div class="item2">
            <a href="#"> <div class="category-women category-d-sm d-flex align-items-end rounded">
              <a href="#">
                <div class="bg-category">Women</div>
              </a>
            </div>
            </a>
          </div>
          <div class="item3">
            <a href="#"> <div class="category-kids category-d-sm d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Kids</div>
              </a>
            </div>
            </a>
          </div>
          <div class="item4">
            <a href="#"> <div class="category-shoes category-d-sm d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Shoes</div>
              </a>
            </div>
            </a>
          </div>
          <div class="item5">
            <a href="#"> <div class="category-hats category-d-sm d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Hats</div>
              </a>
            </div>
            </a>
          </div>
          <div class="item6">
            <a href="#"> <div class="category-sunglasses category-d-sm d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Sunglasses</div>
              </a>
            </div>
            </a>
          </div>
          <div class="item7">
            <a href="#"> <div class="category-watches category-d-sm d-flex align-items-end rounded">
              <a href>
                <div class="bg-category">Watches</div>
              </a>
            </div>
            </a>
          </div>
        </div>
      <!-- </div> -->
    <!-- </div> -->

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
  padding: 0 5px 0 5px;
}

.category-men {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

.category-women {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

.category-kids {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

.category-shoes {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

.category-hats {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

.category-sunglasses {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

.category-watches {
  height: 150px;
  width: 150px;
  background-color: #cccccc;
  padding: 0;
}

/* css grid 2 */

.item1 {
  grid-area: men;
}
.item2 {
  grid-area: women;
}
.item3 {
  grid-area: kids;
}
.item4 {
  grid-area: shoes;
}
.item5 {
  grid-area: hats;
}
.item6 {
  grid-area: sunglasses;
}
.item7 {
  grid-area: watches;
}

.grid-container {
    display: grid;
    grid-template-areas:
    "men women"
    "kids shoes"
    "sunglasses hats"
    "watches watches";
    grid-gap: 5px;
  }

/* .grid-container {
  display: grid;
  grid-template-areas:
    "men women women kids kids "
    "shoes shoes hats kids kids"
    "shoes shoes sunglasses sunglasses watches";
  grid-gap: 5px;
  background-color: #2196f3;
} */



@media only screen and (min-width: 600px) {
  

.grid-container {
  display: grid;
  grid-template-areas:
    "men men women women"
    "kids kids shoes shoes"
    "hats hats sunglasses sunglasses"
    "watches watches watches watches";
  grid-gap: 5px;
  /* background-color: #2196f3; */
  /* padding: 10px; */
}


.category-men {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-women {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-kids {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-shoes {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-hats {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-sunglasses {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-watches {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

}

@media only screen and (min-width: 1100px) {
  

.grid-container {
  display: grid;
  grid-template-areas:
    "men women women kids kids "
    "shoes shoes hats kids kids"
    "shoes shoes sunglasses sunglasses watches";
  grid-gap: 5px;
  
}



.category-men {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-women {
  height: 214px;
  width: 438px;
  background-color: #cccccc;
  padding: 0;
}

.category-kids {
  height: 438px;
  width: 438px;
  background-color: #cccccc;
  padding: 0;
}

.category-shoes {
  height: 438px;
  width: 438px;
  background-color: #cccccc;
  padding: 0;
}

.category-hats {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

.category-sunglasses {
  height: 214px;
  width: 438px;
  background-color: #cccccc;
  padding: 0;
}

.category-watches {
  height: 214px;
  width: 214px;
  background-color: #cccccc;
  padding: 0;
}

}

</style>