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

    <section id="bannerNewCustomerBennefit" class="mt-5">
      <bannerNewCustomer></bannerNewCustomer>
    </section>

    <section id="featuredProducts" class="mt-5">
      <FeaturedProducts></FeaturedProducts>
    </section>

    <section id="flashSales" class="mt-5">
      <BannerFlashSale></BannerFlashSale>
    </section>

    <section id="topSellers" class="mt-5">
      <TopSellers></TopSellers>
    </section>

    <section id="testimonials" class="mt-5">
      <Testimonials></Testimonials>
    </section>

    <section id="latestBlog" class="mt-5">
      <LatestBlog></LatestBlog>
    </section>

    <section id="subscribenow" class="mt-5">
      <SubscribeNow></SubscribeNow>
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

// banner flash sales
import BannerFlashSale from "@/components/banner/BannerFlashSale.vue";

// top sellers  TopSellers
import TopSellers from "@/components/top-sellers/TopSellers.vue";

// Testimonials
import Testimonials from "@/components/testimonials/Testimonials.vue";

// latest blog
import LatestBlog from "@/components/latest-blog/LatestBlog.vue";

// subscribe
import SubscribeNow from "@/components/banner/SubscribeNow.vue";

export default {
  name: "Home",
  components: {
    BannerHome1,
    UserArgument1,
    ShopByCategory1,
    NewArrivals,
    bannerNewCustomer,
    FeaturedProducts,
    BannerFlashSale,
    TopSellers,
    Testimonials,
    LatestBlog,
    SubscribeNow
  },
};
</script>
