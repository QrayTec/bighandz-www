<template>
  <div class="index_First">
    <div class="index_First_Content">
      <div class="index_First_Iamge_title">
        <img src="~/assets/index_image/mian_title.png" alt="">
      </div>
      <div class="index_First_Text_title">常に先へ</div>
      <div class="index_First_Text_content">顧客様より先に考えること | 顧客様より先に行動すること</div>
    </div>
    <div class="Index_scrool">
      <div class="Index_scrool_content">SCROLL</div>
      <div class="Index_scrool_line"></div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style >
.index_First {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  background-image: url('~/assets/index_image/pic_banner.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.index_First_Content {
  width: 1310px;
  margin-top: 80px;
  color: #FFFFFF;
}

.index_First_Iamge_title {
  margin-top: 207px;
}

.index_First_Text_title {
  margin-top: 86px;
  margin-left: 53px;
  font-size: 48px;
  font-family: Noto Sans JP;
  font-weight: bold;
  color: #FFFFFF;
  line-height: 72px;
}

.index_First_Text_content {
  margin-top: 60px;
  margin-left: 55px;
  width: 664px;
  height: 46px;
  background: #597BE5;
  font-size: 24px;
  font-family: Noto Sans JP;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 46px;
  padding: 0 19px;
}
.Index_scrool{
  position: absolute;
  width: 15px;
  height: 152px;
  left: 80px;
  top: 658px;

}
.Index_scrool_content{
  transform: rotate(270deg);
  font-size: 14px;
  font-family: Roboto;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 30px;
}
.Index_scrool_line{
  margin: 20px auto 0;
  width: 1px;
  height: 80px;
  background: linear-gradient(0deg, rgba(255,255,255,0) 0%, #FFFFFF 100%);
}
@media screen and (min-width: 1024px) and (max-width: 1440px) {
 .index_First_Content{
    width: 960px;
  }

  .index_First_Text_title {
    margin-top: 86px;
    margin-left: 60px;
    font-size: 36px;
    font-family: Noto Sans JP;
    font-weight: bold;
    color: #FFFFFF;
    line-height: 72px;
  }
  
  .index_First_Text_content {
    margin-top: 60px;
    margin-left: 60px;
    width: auto;
    height: auto;
    max-width: 453px;
    background: #597BE5;
    font-size: 16px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    padding: 0 19px;
  }
  .Index_scrool {
    position: absolute;
    width: 15px;
    height: 152px;
    left: 30px;
    top: 658px;
}
}

@media screen and (max-width: 1023px) {
  .index_First{
    height: 100vh;
    min-height: 700px;
  }
  .index_First_Iamge_title{
    margin-top: 150px;
  }

  .index_First_Content{
    width: 80%;
  }
  .index_First_Text_title {
    margin-top: 86px;
    margin-left: 22px;
    font-size: 36px;
    font-family: Noto Sans JP;
    font-weight: bold;
    color: #FFFFFF;
    line-height: 72px;
  }
  
  .index_First_Text_content {
    margin-top: 60px;
    margin-left: 22px;
    width: auto;
    height: auto;
    max-width: 453px;
    background: #597BE5;
    font-size: 16px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    padding: 0 19px;
  }
  .Index_scrool {
    position: absolute;
    width: 15px;
    height: 152px;
    left: 10px;
    top: 508px;
}
}
</style>