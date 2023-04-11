<template>
  <div class="NavBar_Index">
    <div class="NavBar_Content">
      <nav class="flex items-center justify-between flex-wrap NavBar_bg">
        <div class="flex items-center flex-shrink-0 text-white mr-6">
          <img src="~/assets/index_image/BigHandzCo.Ltd.png" alt="">
        </div>
        <div class="block lg:hidden">
          <button class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white" @click="isShowList()">
            <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
          </button>
        </div>
        <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto List_NavBar" v-show="NavbarShow">
          <div class="text-sm lg:flex-grow List_NavBar_Main">
            <div class="NavBar_List_Content active_List">
              <NuxtLink to="/" class="active_Text"> 
                ホーム
              </NuxtLink>
            </div>
            <div class="NavBar_List_Content">企業情報</div>
            <div class="NavBar_List_Content">事業概要</div>
            <div class="NavBar_List_Content">採用情報</div>
            <div class="NavBar_List_Content">関連会社</div>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      NavbarShow:false
    }
  },
  mounted(){
    window.addEventListener('resize', this.checkScreenSize)
    this.checkScreenSize()
  },
  methods:{
    isShowList(){
      this.NavbarShow=!this.NavbarShow;
      console.log(this.NavbarShow);
      
    },
    checkScreenSize(){
      if (window.innerWidth < 1024) {
        this.NavbarShow = false
      } else {
        this.NavbarShow = true
      }
    }
  },
  beforeDestroy() {
    window.removeEventListener('resize', this.checkScreenSize)
  }

}
</script>
<style>
  .NavBar_bg{
    height: 80px;
    display: flex;
    justify-content: space-between;
  }
  .NavBar_Index{
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: center;
    background: #0E1B47;

  }
  .NavBar_Content{
    width: 1760px;
  }
  .List_NavBar{
    display: flex;
    justify-content: flex-end;
    align-items: center;

  }
  .List_NavBar_Main{
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  .NavBar_List_Content{
    width: 70px;
    height: 80px;
    font-size: 15px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0px 10px;
  }
  .active_List{
    border-bottom: 4px solid #597BE5;
  }
  .active_Text{
    transform: translateY(4px);
  }
  @media screen and (max-width: 1023px) {
    .NavBar_Index{
      height: auto;
    }
    .NavBar_Content{
      padding: 10px 40px;
    }
    .NavBar_bg{
      height: auto;
    }
    .active_List{
      border-bottom: none;
    }
    .active_Text{
      transform: translateY(0);
    }
    .List_NavBar_Main{
      width: 100%;
      display: flex;
      justify-content: flex-start;
      align-items: center;
      flex-wrap: wrap;
      margin-bottom: 10px;

    }
    .List_NavBar{
      display: flex;
      justify-content: flex-start;
      align-items: center;
      background: #0E1B47;

    }
    .NavBar_List_Content{
      margin-top: 20px;

      width: 100%;
      height: 20px;
      font-size: 15px;
      font-family: Noto Sans JP;
      font-weight: 500;
      color: #FFFFFF;
      display: flex;
      align-items: center;
      justify-content: flex-start;
    }
  }
</style>