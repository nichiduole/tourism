<template>
  <div class="home">
    <home-header></home-header>
    <home-swiper></home-swiper>
    <home-recommend></home-recommend>
  </div>
</template>

<script>
import HomeHeader from './HomeHeader.vue';
import HomeSwiper from './HomeSwiper.vue';
import HomeRecommend from './HomeRecommend.vue';

export default {
  name: "Home",
  components: {
    HomeHeader,
    HomeSwiper,
    HomeRecommend
  },
};
</script>
