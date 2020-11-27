<template>
  <swiper ref="mySwiper" :options="swiperOptions"
  :auto-update="true">
    <swiper-slide>
      <img src="@/assets/swiper/1.png" />
    </swiper-slide>
    <swiper-slide>
      <img src="@/assets/swiper/2.png" />
    </swiper-slide>
    <swiper-slide>
      <img src="@/assets/swiper/3.png" />
    </swiper-slide>
    <swiper-slide>
      <img src="@/assets/swiper/4.png" />
    </swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      swiperOptions: {
        pagination: {
          el: ".swiper-pagination",
        },
        autoplay: {
          delay: 3000,
          disableOnInteraction: false,
        },
        loop: true,
      },
    };
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.$swiper;
    },
  },
};
</script>

<style lang="less">
img {
  width: 100%;
}
.swiper-container{
    --swiper-theme-color: #fff;
  }
</style>
