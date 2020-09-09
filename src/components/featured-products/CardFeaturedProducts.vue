<template>
  <div>
    <!-- d-flex justify-content-center -->
    <!-- <div class="container"> -->
    <div class="item d-flex justify-content-center align-items-center">
      <!-- style="width: 18rem;"                     my-card-style-->
      <div class="card text-center position-relative rounded">
        <div>
          <!--  rounded-circle d-flex justify-content-center-->
          <div class="myBadgeStyle1 d-flex align-items-center justify-content-center " :class="activeClass"
          >{{product.badgeText}}</div>

          <!-- @/assets/Productsleeve.png -->
          <img :src="product.image" class="card-img-top my-img-bg img-fluid" alt="sleeve" />
          <!-- {{product.image}} -->
        </div>
        <!-- Blue silk flare sleeved top -->
        <div class="card-footer myCard-footer text-left rounded-bottom">{{product.name}}</div>

        <!-- overlay content -->
        <div id="my-overlay1" class="d-flex justify-content-start d-flex align-items-end">
          <div class="overlay-content1">
            <div class="text-light head-text">{{product.name}}</div>
            <!-- <div class="btn btn-outline-primary text-light">Fashion</div> -->
            <button
              type="button"
              class="btn btn-sm btn-outline-primary text-light d-flex justify-content-start"
            >Fashion</button>
            <p class="text-light strike d-flex justify-content-start p-0 m-0">
              <s>{{product.targetprice}}</s>
            </p>
            <p class="price d-flex justify-content-start p-0 m-0">{{product.price}}</p>
          </div>

          <div class="mb-4">
            <i class="fas fa-star color-primary"></i>
            <i class="fas fa-star color-primary"></i>
            <i class="fas fa-star color-primary"></i>
            <i class="fas fa-star color-primary"></i>
            <i class="far fa-star color-primary"></i>
          </div>

          <!-- OverLayMenu1 -->
          <div id="overLayMenu1">
            <OverLayMenu1></OverLayMenu1>
          </div>
          <!-- OverLayMenu1 end -->
        </div>
        <!-- overlay content end -->

        <!-- <p>{{activeClass}}</p> -->

      </div>
      <!-- card end -->
    </div>
  </div>

</template>

<script>
import OverLayMenu1 from "@/components/overlay-menu/OverLayMenu1.vue";

export default {
  components: {
    OverLayMenu1,
  },
  props: {
    product: {},
  },

  data() {
    return{
       activeClass: setClassForBadge(this.product.badge),
        danger:false
    }
     
    
  },
  computed:{
    // activeClass=() =>{

    // }
  }
};


// returnerar classnamn för badge
function setClassForBadge(status) {
  switch (status) {
    case "HOT":
      // this.danger=true
      return "badge-danger";
      break;
    case "DISCOUNT":
      return "badge-success";
      break;

    default:
      return "my-badge-color";
      break;
  }
}
</script>

<style scoped>
.my-card-style {
  width: 21.875rem;
  height: 25rem;
}

.myCard-footer {
  background-color: var(--mydark-blue);
  color: var(--white);
  font-size: 18px;
}

.myBadgeStyle1 {
  position: absolute;
  top: 10px;
  left: 10px;
  /* background-color: var(--primaryColor); */
  color: var(--white);
  /* padding: 5px; */
  height: 60px;
  width: 60px;
  border-radius: 50%;
}

.my-badge-color {
  background-color: var(--primaryColor);
}

.my-img-bg {
  background-color: #eeeeee;
}

#my-overlay1 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(31, 48, 143, 0.95);
  /* color: rgb(14, 21, 61); */
  opacity: 0;
  transition: opacity 0.4s;
}
#my-overlay1:hover {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(14, 21, 61, 0.95);
  /* color: rgb(14, 21, 61); */
  opacity: 1;
}

#my-overlay1 .btn {
  border-color: var(--white) !important;
}

#my-overlay1 .btn:hover {
  border-color: rgba(32, 211, 194, 0.2) !important;
  /* border: none; */
  background-color: rgba(32, 211, 194, 0.5) !important;
}

#my-overlay1 .overlay-content1 {
  margin: 0 0 20px 20px;
}

#my-overlay1 .head-text {
  font-size: 18px;
}

#my-overlay1 .price {
  color: var(--primaryColor);
  font-size: 24px;
  font-weight: 700;
}

#overLayMenu1 {
  position: absolute;
  top: 1rem;
  right: 1rem;
}
</style>