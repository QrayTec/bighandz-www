<template>
  <div class="Main_tasks">
    <div class="Main_tasks_content">
      <div class="Main_tasks_Title">
        <h1>主な業務</h1>
      </div>
      <div class="Main_tasks_Cards">
        <div class="Card_1">
          <div>
            <div class="Card_image">
              <img src="~/assets/index_image/icon_kaifayewu.png" alt="">
            </div>
            <div class="Card_Title">
              <p>システム開発</p>
              <p>事業</p>
            </div>
          </div>
        </div>
        <div class="Big_Card_Main">
          <div class="Card_Main">
            <div class="Card_2">
              <div>
                <div class="Card_image_2">
                  <img src="~/assets/index_image/icon_jijianyewu-01.png" alt="">
                </div>
                <div class="Card_Title">
                  <p>インフラ基盤</p>
                  <p>事業</p>
                </div>
              </div>
            </div>
            <div class="Card_3">
              <div class="Card_3_Content">
                <div class="Card_image_3">
                  <img src="~/assets/index_image/icon_jijianyewu-01.png" alt="">
                </div>
                <div class="Card_Title_3">
                  <p class="Card_Main_title">オフショア事業</p>
                  <p class="Card_Main_Content">主な業務経験は製造、流通関係です。</p>
                  <p class="Card_Main_Content">製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</p>
                  <NuxtLink to="/" class="Card_Main_Link">
                    <p>詳細はこちら -></p>
                  </NuxtLink>
              </div>
              </div>
            </div>
           
          </div>
          <div class="Card_Main">
            <div class="Card_4">
              <div>
                <div class="Card_image_4">
                  <img src="~/assets/index_image/icon_zixunyewu-01.png" alt="">
                </div>
                <div class="Card_Title">
                  <p>コンサルテイング事業</p>
                </div>
              </div>
            </div>
            <div class="Card_5">
              <div>
                <div class="Card_image_2">
                  <img src="~/assets/index_image/icon_yiliaobaojianyewu-01.png" alt="">
                </div>
                <div class="Card_Title">
                  <p>ヘルスケア事業</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {

}
</script>
<style>
.m_top_20 {
  margin-top: 20px;
}

.Main_tasks {
  width: 100%;
  height: 920px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.Main_tasks_content {
  width: 1200px;
}
.Main_tasks_Title {
  padding-top: 120px;
}

.Main_tasks_Title h1 {
  font-size: 36px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
}

.Main_tasks_Cards {
  margin-top: 80px;
  display: flex;
  flex-wrap: wrap;
}

.Card_Main {
  height: 287px;
  display: flex;
  flex-wrap: wrap;
}

.Card_1 {
  width: 287px;
  height: 594px;
  background-image: url('~/assets/index_image/pic_Card_1.png');
}

.Big_Card_Main {
  width: 885px;
  height: 594px;
  margin-left: 10px;
}

.Card_2 {
  width: 285px;
  height: 287px;
  background-image: url('~/assets/index_image/pic_Card_2.png');

}

.Card_3 {
  width: 590px;
  height: 287px;
  margin-left: 10px;
  background-image: url('~/assets/index_image/pic_Card_3.png');
  display: flex;
  flex-wrap: wrap;
}

.Card_4 {
  width: 590px;
  height: 287px;
  background-image: url('~/assets/index_image/pic_Card_4.png');
}

.Card_5 {
  width: 285px;
  height: 287px;
  margin-left: 10px;
  background-image: url('~/assets/index_image/pic_Card_5.png');
}

.Card_image {
  margin: 250px 124px 0;
}

.Card_image_2 {
  margin: 102px 123px 0;
}

.Card_image_3 {
  margin-top: 41px;
  margin-left: 41px;
}

.Card_Title {
  font-size: 24px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  text-align: center;
  margin-top: 20px;
}
.Card_Title_3{
  display: flex;
  flex-wrap: wrap;
  max-width: 450px;
  margin-top: 41px;
  margin-left: 20px;

}
.Card_Main_title{
  width: 100%;
  font-size: 24px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 30px;
}
.Card_Main_Content{
  font-size: 18px;
  font-family: Noto Sans JP;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 24px;
}
.Card_Main_Link{
  font-size: 14px;
  font-family: Noto Sans JP;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 72px;
  text-decoration: none;
}
.Card_image_4{
  margin: 103px 275px 0;
}
.Card_3_Content{
  width: 100%;
  display: flex;
  flex-wrap: nowrap;
}
.Card_Main:not(:first-child){
  margin-top: 20px;
}
@media screen and (min-width: 1024px) and (max-width: 1440px) {
  .Card_Main:not(:first-child){
    margin-top: 20px;
  }
  .Card_3_Content{
    width: 100%;
    display: flex;
    flex-wrap: nowrap;
  }
  .Main_tasks{
    height: auto;
  }
  .Main_tasks_content {
    width:960px;
  }
  .Card_1 {
    width: 287px;
    height: 594px;
    background-image: url('~/assets/index_image/pic_Card_1.png');
  }
  
  .Big_Card_Main {
    width: 620px;
    height: 594px;
    margin-left: 10px;
  }
  
  .Card_2 {
    width: 200px;
    height: 287px;
    background-image: url('~/assets/index_image/pic_Card_2.png');
  
  }
  
  .Card_3 {
    width: 410px;
    height: 287px;
    margin-left: 10px;
    background-image: url('~/assets/index_image/pic_Card_3.png');
    display: flex;
    flex-wrap: wrap;
  }
  
  .Card_4 {
    width: 410px;
    height: 287px;
    background-image: url('~/assets/index_image/pic_Card_4.png');
  }
  
  .Card_5 {
    width: 200px;
    height: 287px;
    margin-left: 10px;
    background-image: url('~/assets/index_image/pic_Card_5.png');
  }
  
  .Card_image {
    margin: 250px 124px 0;
  }
  
  .Card_image_2 {
    margin: 71px 80px 0;
  }
  .Card_image_2 img{
    width: 40px;
    height: 40px;
  }
  
  .Card_image_3 {
    margin-top: 40px;
    margin-left: 20px;
  }
  
  .Card_Title {
    font-size: 24px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    text-align: center;
    margin-top: 20px;
  }
  .Card_Title_3{
    display: flex;
    flex-wrap: wrap;
    max-width: 310px;
    margin-top: 41px;
    margin-left: 20px;
  
  }
  .Card_Main_title{
    width: 100%;
    font-size: 24px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    line-height: 30px;
  }
  .Card_Main_Content{
    font-size: 18px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 24px;
  }
  .Card_Main_Link{
    font-size: 14px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 72px;
    text-decoration: none;
  }
  .Card_image_4{
    margin:71px 185px 0;
  }
}
@media screen and (min-width: 762px) and (max-width: 1023px){
  .Main_tasks{
    height: auto;
  }
  .Main_tasks_content {
    width:80%;
  }
  .Big_Card_Main {
    width: 620px;
    height: auto;
    margin-top: 0px;
    margin-left: 0;

  }
  .Main_tasks_Cards{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .Card_Main{
    width: auto;
    height: 300px;
    display: flex;
    justify-content: center;
    margin-top: 20px;

  }
  .m_top_20{
    margin-top: 0;
  }
  .Card_1 {
    width: 620px;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_1.png');

  }
  .Card_2 {
    width: 300px;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_2.png');
  
  }
  
  .Card_3 {
    width: 300px;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_3.png');
  
  }
  .Card_3_Content{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
  }
  .Card_4 {
    width: 300px;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_4.png');
  }
  
  .Card_5 {
    width: 300px;
    height: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_5.png');
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
  }
  
  .Card_image {
    width: 100%;
    margin: 0;
    display: flex;
    justify-content: center;
  }

  .Card_image_2 {
    width: 100%;
    height: 40px;
    margin:  0;
    display: flex;
    justify-content: center;
  }
  
  .Card_image_3 {
    margin-top: 0;
    margin-left: 0;
  }
  
  .Card_Title {
    width: 100%;
    font-size: 24px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    text-align: center;
    margin-top: 20px;
  }
  .Card_Title_3{
    display: flex;
    flex-wrap: wrap;
    width: 100%;
    max-width: 310px;
    margin-top: 10px;
    margin-left: 0px;
    justify-content: center;
    align-items: center;
    text-align: center;
  
  }
  .Card_Main_title{
    width: 100%;
    font-size: 24px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    line-height: 30px;
  }
  .Card_Main_Content{
    font-size: 18px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 24px;
  }
  .Card_Main_Link{
    font-size: 14px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 25px;
    text-decoration: none;
  }
  .Card_image_4{
    margin: 0;
    display: flex;
    justify-content: center;
  }
}
@media screen and (max-width: 762px) {

  .Main_tasks{
    height: auto;
  }
  .Main_tasks_content {
    width:80%;
  }
  .Big_Card_Main {
    width: 620px;
    height: auto;
    margin-top: 0px;
    margin-left: 0;

  }
  .Main_tasks_Cards{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .Card_Main{
    width: auto;
    display: flex;
    justify-content: center;
  }
  .Card_1 {
    width: 300px;
    height: 300px;
    padding: 0px 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_1.png');

  }
  .Card_2 {
    width: 300px;
    height: 300px;
    padding: 0px 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_2.png');
    margin-top: 20px;
  
  }
  
  .Card_3 {
    width: 300px;
    height: 300px;
    padding: 0px 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_3.png');
    margin-left: 0;
    margin-top: 20px;

  
  }
  .Card_3_Content{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
  }
  .Card_4 {
    width: 300px;
    height: 300px;
    padding: 0px 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_4.png');
    margin-top: 20px;

  }
  
  .Card_5 {
    width: 300px;
    height: 300px;
    padding: 0px 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    background-size: cover;
    background-position: center;
    background-image: url('~/assets/index_image/pic_Card_5.png');
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin-left: 0px;
    margin-top: 20px;
  }
  
  .Card_image {
    width: 100%;
    margin: 0;
    display: flex;
    justify-content: center;
  }
  
  .Card_image_2 {
    width: auto;
    height: auto;
    margin: 0;
    display: flex;
    justify-content: center;
  }
  
  .Card_image_3 {
    margin-top: 40px;
    margin-left: 20px;
  }
  
  .Card_Title {
    width: 100%;
    font-size: 24px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    text-align: center;
    margin-top: 20px;
  }
  .Card_Title_3{
    display: flex;
    flex-wrap: wrap;
    width: 100%;
    max-width: 310px;
    margin-top: 10px;
    margin-left: 0px;
    justify-content: center;
    align-items: center;
    text-align: center;
  
  }
  .Card_Main_title{
    width: 100%;
    font-size: 18px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    line-height: 30px;
  }
  .Card_Main_Content{
    font-size: 18px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 24px;
  }
  .Card_Main_Link{
    font-size: 14px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 20px;
    text-decoration: none;
  }
  .Card_image_4{
    margin:0;
    display: flex;
    justify-content: center;
  }
  .Card_Main{
    height: auto;
  }
}
</style>