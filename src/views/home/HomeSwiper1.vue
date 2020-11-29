<template>
<div>
  <swiper ref="mySwiper" v-for="(leaf,index) in leaves" :key="index" class="recommend">
    <swiper-slid v-for="png in leaf" :key="png.id" class="column">
        <img :src="png.imgUrl" />
    </swiper-slid>
  </swiper>
</div>
</template>

<script>
export default {
  name: "HomeSwiper1",
  data() {
    return {
      pngs: [
        {
          id: 0,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 1,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 2,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 3,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 4,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 5,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 6,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 7,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },{
          id: 8,
          imgUrl: 'https://s.qunarzz.com/homenode/images/touchheader/hotel.png',
        },
      ],
    };
  },
  computed: {
    swiper() {
      return this.$refs.mySwiper.$swiper;
    },
    leaves() {
      const leaves = [];
      this.pngs.forEach(png => {
        const leaf = Math.floor(png.id / 8);
        if(!leaves[leaf]) {
          leaves[leaf] = []
        }
        leaves[leaf].push(png)
      })
      return leaves
    }
  },
};
</script>

<style lang="less" scoped>
.recommend {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    text-align: center;
    padding-top: 10px;
    background-color: rgba(255,207,72,.1);
  }
  .column {
    flex: 25%;
    img {
      width: 40px;
      // margin-bottom: -15px;
    }
  }
.swiper-container{
    --swiper-theme-color: #fff;
  }
</style>
