<template>
  <div class="home">
    <home-header></home-header>
    <home-swiper></home-swiper>
  </div>
</template>

<script>
import HomeHeader from './HomeHeader.vue';
import HomeSwiper from './HomeSwiper.vue'
export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper
  },
};
</script>
