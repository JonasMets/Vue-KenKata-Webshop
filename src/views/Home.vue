<template>
  <div class="home">

    <section id="bannerHome">
      <BannerHome1></BannerHome1>
    </section>
    <section id="userargument1">
      <UserArgument1></UserArgument1>
    </section>

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import BannerHome1 from "@/components/banner/BannerHome1.vue";
import UserArgument1 from "@/components/why-use-our-site/UserArgument1.vue";

export default {
  name: "Home",
  components: {
    BannerHome1,
    UserArgument1
  },
};
</script>
