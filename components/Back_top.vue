<template>
  <div class="Back_Top" @click="Back_top" v-show="showBackTop">
    <img src="~/assets/index_image/icon_top-01.png" alt="">
  </div>
</template>
<script>
export default {
  data() {
    return {
      showBackTop: false // 是否显示返回顶部按钮
    }
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  methods:{
    handleScroll() {
      if (window.pageYOffset > 0) {
        this.showBackTop = true;
      } else {
        this.showBackTop = false;
      }
    },
    Back_top(){
      window.removeEventListener("scroll", this.handleScroll);
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
      this.showBackTop=false;
      setTimeout(() => {
        window.addEventListener("scroll", this.handleScroll);
      }, 1000);
    }
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.handleScroll);
  }
}
</script>
<style>
  .Back_Top{
    width: 70px;
    height: 70px;
    cursor: pointer;
    background: #576CB0;
    position: fixed;
    right: 0px;
    bottom: 150px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  @media only screen and (max-width: 768px){
    .Back_Top{
      width: 40px;
      height: 40px;
    }
  }
</style>