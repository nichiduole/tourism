<template>
  <div class="home">
    <home-header></home-header>
    <home-swiper></home-swiper>
    <!-- <home-swiper1></home-swiper1> -->
    <home-recommend></home-recommend>
    <home-travels></home-travels>
  </div>
</template>

<script>
import HomeHeader from './HomeHeader.vue';
import HomeSwiper from './HomeSwiper.vue';
// import HomeSwiper1 from './HomeSwiper1.vue';
import HomeRecommend from './HomeRecommend.vue';
import HomeTravels from './HomeTravels.vue';

export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper,
    // HomeSwiper1,
    HomeRecommend,
    HomeTravels,
  },
};
</script>
