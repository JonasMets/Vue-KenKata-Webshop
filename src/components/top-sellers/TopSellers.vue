<template>
  <div>
    <!-- overhead text -->
    <div class="container mt-5 justify-content-center text-center">
      <div class="row">
        <div class="col">
          <div class="d-flex justify-content-center font-play">
            <h2 class="fs-36 font-weight-bolder">
              TOP
              <span class="color-primary fs-36 font-weight-bolder">SELLERS</span>
            </h2>
          </div>
          <div class="d-flex justify-content-center">
            <img src="@/assets/wave.png" alt class />
          </div>
          <!-- -->
          <div class="d-flex justify-content-center">
            <p>Check out our weekly top sellers in all category</p>
          </div>
        </div>
      </div>
    </div>

    <div class="container">
      <div class="row align-items-center">
        <div class="col-6">
          <div class="my-img1 h-100">
            <CardTopSellers :product="newProducts[0]" />
          </div>
        </div>
        <div class="col-6">
          <div class="row">
            <div class="col-12">
              <div class="my-img2 h-100">
                <CardTopSellers :product="newProducts[1]" />
              </div>
            </div>
            <div class="col-12">
              <div class="my-img3 h-100">
                <CardTopSellers :product="newProducts[2]" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardTopSellers from "@/components/top-sellers/CardTopSellers.vue";

export default {
  components: {
    CardTopSellers,
  },
  data() {
    return {
      newProducts: [
        {
          category: "Outwear",
          name: "Men's denim shirts full",
          targetprice: "$25",
          price: "$19.00",
          badge: "",
          badgeText: "HOT",
          image: require("@/assets/MensDenim.png"),
          rating: 5,
        },
        {
          category: "Accessories",
          name: "Women's leather bag and shoe",
          targetprice: "$220",
          price: "$190.00",
          badge: "NEW",
          badgeText: "NEW",
          image: require("@/assets/WomensBag.png"),
          rating: 5,
        },
        {
          category: "Outwear",
          name: "New look men's sneakers",
          targetprice: "$120",
          price: "$99",
          badge: "DISCOUNT",
          badgeText: "-30%",
          image: require("@/assets/MensSneakers.png"),
          rating: 5,
        },
        {
          category: "Outwear",
          name: "Black jacket",
          targetprice: "$200",
          price: "$150",
          badge: "NEW",
          badgeText: "NEW",
          image: require("@/assets/MensCoat.png"),
          rating: 5,
        },
      ],
    };
  },
};
</script>

<style scoped>
.my-img1 {
  width: 100%;
  max-height: 700px;
}
.my-img2 {
  max-height: 345px;
}
.my-img3 {
  max-height: 345px;
}
</style>