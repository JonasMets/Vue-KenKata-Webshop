<template>
  <div class="home">
    <section id="bannerHome">
      <BannerHome1></BannerHome1>
    </section>
    <section id="userArgument1">
      <UserArgument1></UserArgument1>
    </section>

    <section id="shopByCategory">
      <!-- <ShopByCategory1></ShopByCategory1> -->
      <!-- test -->
      <ShopByCategory12></ShopByCategory12>
      <!-- test -->
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import BannerHome1 from "@/components/banner/BannerHome1.vue";
import UserArgument1 from "@/components/why-use-our-site/UserArgument1.vue";
// import ShopByCategory1 from "@/components/shop-by-category/ShopByCategory1.vue";
import ShopByCategory12 from "@/components/shop-by-category/ShopByCategory1_2.vue";

export default {
  name: "Home",
  components: {
    BannerHome1,
    UserArgument1,
    // ShopByCategory1,
    ShopByCategory12
  },
};
</script>
