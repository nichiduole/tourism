<template>
  <div class="header">
    <div class="left">
      <img src="~@/assets/home/header/1.png" alt="">
    </div>
    <div class="input">
      <i></i>
      <input type="text" placeholder="请输入目的地">
    </div>
    <div class="right">搜索
      <img src="~@/assets/home/header/3.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeHeader",
};
</script>

<style lang="less">
  .header {
    display: flex;
    background-color: #FFD000;
    height: 44px;
    line-height: 44px;
    color: #fff;
  }
  .left {
    width: 40px;
    text-align: center;
    
    img {
      vertical-align: middle;
      width: 24px;
      height: 24px;
    }
  }
  .input {
    flex: 1;
    background-color: #fff;
    border-radius: 5px;
    height: 30px;
    line-height: 30px;
    margin-top: 7px;
    i::before {
      content: '';
      display: inline-block;
      background: url(~@/assets/home/header/2.png) no-repeat;
      background-size: cover;
      width: 16px;
      height: 16px;
      margin-left: 10px;
      vertical-align: middle;
      margin-bottom: 1px;
    }
    input {
      margin-left: 7px;
      border: none;
      font-size: 14px;
    }
  }
  .right {
    width: 60px;
    text-align: center;
    img {
      width: 20px;
      height: 20px;
      vertical-align: middle;
      margin: -5px 0 0 -5px;
    }
  }
</style>
