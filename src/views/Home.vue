<template>
  <div class="home">
    <section id="bannerHome">
      <BannerHome1></BannerHome1>
    </section>
    <section id="userArgument1">
      <UserArgument1></UserArgument1>
    </section>

    <section id="shopByCategory">
      <ShopByCategory1></ShopByCategory1>
    </section>

    <section id="neWArrivals">
      <NewArrivals></NewArrivals>
    </section>

    <section id="bannerNewCustomerBennefit">
      <bannerNewCustomer></bannerNewCustomer>
    </section>


    <section id="featuredProducts">
      <FeaturedProducts></FeaturedProducts>
    </section>

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import BannerHome1 from "@/components/banner/BannerHome1.vue";
import UserArgument1 from "@/components/why-use-our-site/UserArgument1.vue";
// import ShopByCategory1 from "@/components/shop-by-category/ShopByCategory1.vue";
import ShopByCategory1 from "@/components/shop-by-category/ShopByCategory1.vue";
// 
// import NewArrivals from "@/components/newarrivals/NewArrivals.vue";
import NewArrivals from "@/components/newarrivals/NewArrivalsV2.vue";
// 
import bannerNewCustomer from "@/components/banner/bannerNewCustomerBennefit1.vue";

// featured products
import FeaturedProducts from "@/components/featured-products/FeaturedProducts.vue";

export default {
  name: "Home",
  components: {
    BannerHome1,
    UserArgument1,
    ShopByCategory1,
    NewArrivals,
    bannerNewCustomer,
    FeaturedProducts
  },
};
</script>
