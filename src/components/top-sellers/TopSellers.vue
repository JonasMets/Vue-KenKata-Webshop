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

          <div class="d-none d-block d-sm-none">
            <button class="btn rounded-pill color-primary my-bg-primary text-light">Show</button>
          </div>

        </div>
      </div>
    </div>

    <div class="container">
      <div class="row align-items-center justify-content-center">
        <div class="col-6 d-none d-lg-block">
          <div class="my-img1">
            <CardTopSellers :product="newProducts[0]" />
          </div>
        </div>
        <div class="col-6 d-none d-lg-block">
          <div class="row d-flex flex-column">
            <div class="col">
              <div class="my-img2">
                <CardTopSellers :product="newProducts[1]" />
              </div>
            </div>
            <div class="col">
              <div class="my-img3">
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
          badgeText: "",
          logo: require("@/assets/BeximSmall.png"),
          image: require("@/assets/MensDenim.png"),
          rating: 5,
        },
        {
          category: "Accessories",
          name: "Women's leather bag and shoe",
          targetprice: "$220",
          price: "$190.00",
          badge: "",
          badgeText: "",
          logo: require("@/assets/LightonSmall.png"),
          image: require("@/assets/WomensBag.png"),
          rating: 5,
        },
        {
          category: "Shoes",
          name: "New look men's sneakers",
          targetprice: "$120",
          price: "$99",
          badge: "",
          badgeText: "",
          logo: require("@/assets/RosimoSmall.png"),
          image: require("@/assets/MensSneakers3.png"),
          rating: 5,
        },
        {
          category: "Outwear",
          name: "Black jacket",
          targetprice: "$200",
          price: "$150",
          badge: "",
          badgeText: "",
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
  /* min-width: 550px; */
  max-height: 700px;
}
.my-img2 {
  /* width: 100%; */
  max-height: 345px;
}
.my-img3 {
  /* width: 100%; */
  max-height: 345px;
}
</style>