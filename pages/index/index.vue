<template>
  <div class="Index">
    <header>
      <HeaderNavBar class="Header"></HeaderNavBar>
    </header>
    <main>
      <section>
        <!-- Index_First -->
        <IndexFirst></IndexFirst>
      </section>
      <section>
        <div class="Main_background">
            <!-- Main tasks. -->
          <MainTasks></MainTasks>
          <IndustryArea></IndustryArea>
        </div>
        
      </section>
      <section>
        <MajorClients></MajorClients>
      </section>
    </main>
    <footer>
      <Footer></Footer>
    </footer>
    <BackTop></BackTop>
  </div>
</template>
<script>
export default {

}
</script>
<style>
* {
  margin: 0;
  padding: 0;
}
.Header{
  position: fixed;
  left: 0;
  right: 0;
  z-index: 999;
}
.First_data {
  width: 100%;
  height: 100vh;
  overflow: hidden;

}

.bg {
  width: 100%;
  height: 100%;
  z-index: -1;
  background-image: url('~/assets/index_image/pic_banner.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.First_data_main{
  z-index: 1;
  padding: 80px 80px 0px;
}
.Mian_title{
  margin: 207px 0 0 225px;
}
.Mian_title_text{
  height: 46px;
  font-size: 48px;
  font-weight: bold;
  color: #FFFFFF;
  margin-top: 86px;
  margin-left: 278px;
}
.First_data_Content{
  width: 667px;
  background: #597BE5;
  font-size: 24px;
  font-weight: 400;
  color: #FFFFFF;
  margin-top: 60px;
  margin-left: 280px;
  padding: 9px 23px 9px 19px;

}
.Mian_scrool_content{
  width: 11px;
  height: 52px;
  font-size: 14px;
  font-family: Roboto;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 30px;
  transform: rotate(270deg);
}
.Mian_scrool_line{
  width: 1px;
  height: 80px;
  background: linear-gradient(0deg, rgba(255,255,255,0) 0%, #FFFFFF 100%);
  transform: translateX(-5px);
}
.Main_background{
  width: 100%;
  height: 1260px;
  background: linear-gradient(0deg, #0E1B47 0%, #2E4A9E 100%);
}
@media screen and (min-width: 1024px) and (max-width: 1440px){
  .Main_background{
    height: auto;
  }
}
@media screen and (max-width: 1023px) {
  .Main_background{
    height: auto;
  }
}
</style>