<template>
  <div class="Header">
    <div class="HeaderMain">
      <div class="header_logo">
        <NuxtLink to="/">
          <img src="~/assets/index_image/BigHandzCo.Ltd.png" alt="">
        </NuxtLink>
      </div>
      <client-only >
        <el-menu :default-active="activeIndex" class="el-menu-demo display" mode="horizontal" :ellipsis="false"
          @select="handleSelect" background-color="#0E1B47" text-color="#FFFFFF" active-text-color="#ffffff" >
          <div class="flex-grow" />
            <el-menu-item index="0">ホーム</el-menu-item>
            <el-menu-item index="1">企業情報</el-menu-item>
            <el-menu-item index="2">事業概要</el-menu-item>
            <el-menu-item index="3">採用情報</el-menu-item>
            <el-menu-item index="4">関連会社</el-menu-item>
        </el-menu>
      </client-only>
      <div class="PhoneNavBar">
          <div>X</div>
      </div>
    </div>
  </div>
</template>
  
<script>
import { ref } from 'vue'

export default {
  data() {
    return {
      activeIndex: ref('0'),
    }
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>
  
<style>
* {
  margin: 0;
  padding: 0;
}
.PhoneNavBar{
  display: none;
}
.Header {
  width: 100%;
  height: 80px;
  position: fixed;
  top: 0;
  left: 0;
  background-color: #0E1B47;
  z-index: 100;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header_logo{
  margin-left: 80px;
}
.HeaderMain{
  width: 100%;
  padding: 10px 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;

}
.flex-grow {
  flex-grow: 1;
}

.el-menu-demo {
  width: 100%;
  height: 80px;
  margin-right: 80px;
}

.header_logo img {
  width: 68px;
  height: 48px;
  margin: 16px 0px;
}

.el-menu-item {
  width: 70px;
  margin: 0px 20px;
}

.el-menu--horizontal>.el-menu-item.is-active {
  border-bottom: 4px solid #597BE5;
  margin: 0px 20px;
}

.el-menu--horizontal>.el-menu-item {
  margin: 0px 20px;

}

.el-menu--horizontal {
  border: none;
}
@media only screen and (max-width: 600px){
  .display{
    display: none;
  }
  .PhoneNavBar{
    display: block;
    color: white;
  }
  .header_logo{
    margin: 0;
  }
  .Header{
    height: 60px;
  }
  .HeaderMain{
    width: 100%;
    padding: 10px 20px;
    display: flex;
    align-items: center;
    justify-content: space-between;

  }
}
</style>
  