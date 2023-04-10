<template>
  <div class="Index">
    <header>
      <Header></Header>
    </header>
    <main>
      <section>
        <div class="First_data">
          <div class="bg">
            <div class="First_data_main">
              <div class="First_Main_title">
                <div class="Mian_title">
                  <img src="~/assets/index_image/mian_title.png" alt="">
                </div>
                <div class="Mian_title_text">常に先へ</div>
                <div class="First_data_Content">
                  顧客様より先に考えること | 顧客様より先に行動すること
                </div>
                <div class="Mian_scrool">
                  <div class="Mian_scrool_content">SCROLL</div>
                  <div class="Mian_scrool_line"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
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

.First_data {
  width: 100%;
  height: 920px;
  overflow: hidden;

}

.bg {
  width: 100%;
  height: 920px;
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
.Mian_scrool{

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
</style>