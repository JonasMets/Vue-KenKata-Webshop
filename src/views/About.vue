<template>
  <div class="about">
    <section id="bannerAbout1">
      <BannerWeAreShop></BannerWeAreShop>
    </section>

    <section id="about-video1">
      <ResposnibleOnlineStore></ResposnibleOnlineStore>
    </section>

    <section id="About-subscribenow" class="mt-5">
      <SubscribeNow></SubscribeNow>
    </section>
  </div>
</template>


<script>
// banner about
import BannerWeAreShop from "@/components/banner/BannerWeAreShop.vue";
// subscribe
import SubscribeNow from "@/components/banner/SubscribeNow.vue";
// video
import ResposnibleOnlineStore from "@/components/responsible-online-store/ResposnibleOnlineStore.vue";

export default {
  name: "About",
  components: {
    BannerWeAreShop,
    SubscribeNow,
    ResposnibleOnlineStore
  },
};
</script>

<style scoped>
</style>
