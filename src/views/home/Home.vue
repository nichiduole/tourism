<template>
  <div class="home">
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-recommend></home-recommend>
    <home-travels></home-travels>
    getData()
  </div>
</template>

<script>
import HomeHeader from './HomeHeader.vue';
import HomeSwiper from './HomeSwiper.vue';
import HomeRecommend from './HomeRecommend.vue';
import HomeTravels from './HomeTravels.vue';

export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper,
    HomeRecommend,
    HomeTravels,
  },
};
</script>
