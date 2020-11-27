<template>
  <div class="recommend">
    <div class="column">
      <img src="~@/assets/home/recommend/1.png">
      <p>指南</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/2.png">
      <p>风景</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/3.png">
      <p>美食</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/4.png">
      <p>酒店</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/5.png">
      <p>交通</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/6.png">
      <p>地图</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/7.png">
      <p>行李</p>
    </div>
    <div class="column">
      <img src="~@/assets/home/recommend/8.png">
      <p>摄影</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data() {
    return {
      
    }
  }
}
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
      margin-bottom: -15px;
    }
  }
</style>
