<template>
  <div id="Home">
    <div class="xunyanji_top">
      <div class="logo" :style="{'background-image': 'url(' + require('./assets/img/top1.png') + ')'}">
        <img src="./assets/img/1.png" alt="">
        <img src="./assets/img/chuban.png" alt="">
      </div>
      <div class="top" :style="{'background-image': 'url(' + require('./assets/img/top2.png') + ')'}">
        <img src="./assets/img/select.png" alt="">
      </div>
      <div class="notice" :style="{'background-image': 'url(' + require('./assets/img/3-3.png') + ')'}">
          <div><img src="./assets/img/lieri.png"></div>
      </div>
      <div class="apply">
          <img src="./assets/img/4-4-1.png" alt="" style="width:50%;height:100%;display:inline-block;">
          <img src="./assets/img/4-4-2.png" alt="" style="width:50%;height:100%;display:inline-block;">
      </div>
      <div>
        <router-link to="/about">点击报名</router-link>
        <router-link to="/about">为她投票</router-link>
      </div>
    </div>
    <!-- <router-view></router-view> -->
  </div>
</template>

<script>
  import Hello from './components/Hello'
  import Vheader from './components/Vheader'
export default {
  name: 'Home',
  components: {
    Hello,
    Vheader
  }
}
</script>

<style>
#Home {
  margin: 0 auto;
  padding: 0;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
img{
  display: block;
  width:100%;
  height:auto;
}
.xunyanji_top{
  margin: 0 auto;
  padding: 0;
}
.logo,.top,.notice,.apply{
  background-size:100% 100%;
}
.apply{
  display: flex;
}
.apply img{
  width:auto;
  flex:1;
}


</style>
