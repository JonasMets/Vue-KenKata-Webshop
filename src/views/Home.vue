<template>
  <div class="home">
    
    <!-- <div class="" style="color:blue;text-align:center;  height:200px;">
      <h3 style="margin-top:100px;">ta bort div i Home.vue efter test</h3> 
    </div> -->
    <BannerHome1></BannerHome1>


  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import  BannerHome1 from '@/components/banner/BannerHome1.vue';

export default {
  name: 'Home',
  components: {
    BannerHome1
  }
}
</script>
