<template>
  <div class="Main_tasks">
    <div class="Main_tasks_content">
      <div class="Main_tasks_Title">
        主な業務
      </div>
      <div class="Main_tasks_Card">
        <div class="Card_1">
          <div class="Card_Image_1">
            <div class="Card_1_Content animate__fadeInUp animate__animated">
              <div class="Card_Image_Icon">
                <img src="~/assets/index_image/icon_kaifayewu.png" alt="icon_kaifayewu">
              </div>
              <div class="Card_Title">
                システム開発
              </div>
              <div class="Card_Text animate__fadeInUp animate__animated animate-hover">
                <p>主な業務経験は製造、流通関係です。</p>
                <p>製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</p>
                <p><nuxt-link to="/">詳細はこちら -></nuxt-link></p>
              </div>
            </div>
          </div>
        </div>
        <div>
          <div class="Card_2">
            <div class="Card_Image_2">
              <div class="Card_1_Content animate__fadeInUp animate__animated">
                <div class="Card_Image_Icon">
                  <img src="~/assets/index_image/icon_jijianyewu-01.png" alt="icon_kaifayewu">
                </div>
                <div class="Card_Title">
                  システム開発
                </div>
                <div class="Card_Text animate__fadeInUp animate__animated animate-hover">
                  <p>主な業務経験は製造、流通関係です。</p>
                  <p>製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</p>
                  <p><nuxt-link to="/">詳細はこちら -></nuxt-link></p>
                </div>
              </div>
            </div>
            <div class="Card_Image_3">
              <div class="Card_1_Content animate__fadeInUp animate__animated">
                <div class="Card_Image_Icon1 ">
                  <img src="~/assets/index_image/icon_lianyewu-01.png" alt="icon_kaifayewu">
                </div>
                <div class="Card3_Content">
                  <div class="Card_Title">
                    システム開発
                  </div>
                  <div class="Card_Text animate__fadeInUp animate__animated animate-hover">
                    <p>主な業務経験は製造、流通関係です。</p>
                    <p>製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</p>
                    <p><nuxt-link to="/">詳細はこちら -></nuxt-link></p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="Card_2">
            <div class="Card_Image_4">
              <div class="Card_1_Content animate__fadeInUp animate__animated">
                <div class="Card_Image_Icon1 ">
                  <img src="~/assets/index_image/icon_zixunyewu-01.png" alt="icon_kaifayewu">
                </div>
                <div class="Card3_Content">
                  <div class="Card_Title">
                    システム開発
                  </div>
                  <div class="Card_Text animate__fadeInUp animate__animated animate-hover">
                    <p>主な業務経験は製造、流通関係です。</p>
                    <p>製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</p>
                    <p><nuxt-link to="/">詳細はこちら -></nuxt-link></p>
                  </div>
                </div>
              </div>
            </div>
            <div class="Card_Image_5">
              <div class="Card_1_Content animate__fadeInUp animate__animated">
                <div class="Card_Image_Icon">
                  <img src="~/assets/index_image/icon_yiliaobaojianyewu-01.png" alt="icon_kaifayewu">
                </div>
                <div class="Card_Title">
                  システム開発
                </div>
                <div class="Card_Text animate__fadeInUp animate__animated animate-hover">
                  <p>主な業務経験は製造、流通関係です。</p>
                  <p>製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</p>
                  <p><nuxt-link to="/">詳細はこちら -></nuxt-link></p>
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
  mounted() {

  }
}
</script>
<style>
.Main_tasks {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
}

.Main_tasks_content {
  width: 1200px;
  height: 920px;
  padding-top: 120px;
}

.Main_tasks_Title {
  font-size: 36px;
  font-family: 'Roboto', 'Noto Sans JP', sans-serif;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 72px;
}

.Main_tasks_Card {
  margin-top: 80px;
  display: flex;
}

.Card_1 {
  width: 287px;
  height: 594px;
}

.Card_2 {
  width: 893px;
  height: 287px;
  display: flex;
  margin-left: 20px;
}

.Card_Image_1 {
  width: 287px;
  height: 594px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  background-image: url('~/assets/index_image/pic_Card_1.png');
}

.Card_Image_2 {
  width: 287px;
  height: 287px;
  padding: 20px 0;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  background-image: url('~/assets/index_image/pic_Card_2.png');
}

.Card_Image_3 {
  width: 590px;
  height: 287px;
  margin-left: 20px;
  padding: 20px 40px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  background-image: url('~/assets/index_image/pic_Card_3.png');
}

.Card_Image_4 {
  width: 590px;
  height: 287px;
  padding: 20px 0;
  margin-top: 20px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  background-image: url('~/assets/index_image/pic_Card_4.png');
}

.Card_Image_5 {
  width: 287px;
  height: 287px;
  padding: 20px 0;
  margin-top: 20px;
  margin-left: 20px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  background-image: url('~/assets/index_image/pic_Card_5.png');
}

.Card_1_Content {
  width: 100%;
  height: 100px;
  transition: height 0.3s ease-out;
}

.Card_Image_Icon {
  width: 100%;
  display: flex;
  justify-content: center;
}

.Card3_Content {
  display: flex;
  flex-wrap: wrap;
}

.Card_Title {
  width: 100%;
  height: auto;
  font-size: 24px;
  font-family: 'Roboto', 'Noto Sans JP', sans-serif;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 30px;
  margin-top: 10px;
  display: flex;
  justify-content: center;
}

.Card_Text {
  padding: 0px 20px;
  font-size: 18px;
  font-family: 'Roboto', 'Noto Sans JP', sans-serif;
  font-weight: 400;
  color: #FFFFFF;
  line-height: 24px;
  display: none;
  transition: all 1s linear;
}

.Card_Text p {
  margin-top: 10px;
}

.Card_Image_1:hover .Card_Text {
  display: block;
  transition: transform 1s linear 0s;

}

.Card_Image_1:hover .Card_1_Content {
  height: 280px;
}

.Card_Image_2:hover .Card_Text {
  display: block;

}

.Card_Image_2:hover .Card_1_Content {
  height: 280px;
}

.Card_Image_Icon1 {
  width: 100%;
  display: flex;
  justify-content: center;
  transition: all 1s ease;

}

.Card_Image_3:hover .Card_Image_Icon1 {
  width: 40px;
  height: 40px;
  margin-top: 20px;
  transition: all 1s ease;
}

.Card_Image_3:hover .Card_1_Content {
  height: 280px;
  display: flex;
  flex-wrap: nowrap;
  margin-left: 20px;

}

.Card_Image_3:hover .Card3_Content {
  width: 420px;
  height: 250px;
  display: flex;
  flex-wrap: wrap;
  margin-left: 20px;
  align-items: self-start;
}

.Card_Image_3:hover .Card_Title {
  width: auto;
  height: 24px;
  line-height: 24px;
  margin-top: 20px;
  transition: transform 1s linear 0s;
}

.Card_Image_3:hover .Card_Text {
  display: block;
  padding: 0px;
  transition: transform 1s linear 0s;
}

.Card_Image_3:hover .Card_Image_Icon1 {
  width: 40px;
  height: 40px;
  margin-top: 20px;
  transition: all 1s ease;
}

.Card_Image_3:hover .Card_1_Content {
  height: 280px;
  display: flex;
  flex-wrap: nowrap;
  margin-left: 20px;

}

.Card_Image_3:hover .Card3_Content {
  width: 420px;
  height: 250px;
  display: flex;
  flex-wrap: wrap;
  margin-left: 20px;
  align-items: self-start;
}

.Card_Image_3:hover .Card_Title {
  width: auto;
  height: 24px;
  line-height: 24px;
  margin-top: 20px;
  transition: transform 1s linear 0s;
}

.Card_Image_3:hover .Card_Text {
  display: block;
  padding: 0px;
  transition: transform 1s linear 0s;
}


.Card_Image_4:hover .Card_Image_Icon1 {
  width: 40px;
  height: 40px;
  margin-top: 20px;
  transition: all 1s ease;
}

.Card_Image_4:hover .Card_1_Content {
  height: 280px;
  display: flex;
  flex-wrap: nowrap;
  margin-left: 20px;

}

.Card_Image_4:hover .Card3_Content {
  width: 420px;
  height: 250px;
  display: flex;
  flex-wrap: wrap;
  margin-left: 20px;
  align-items: self-start;
}

.Card_Image_4:hover .Card_Title {
  width: auto;
  height: 24px;
  line-height: 24px;
  margin-top: 20px;
  transition: transform 1s linear 0s;
}

.Card_Image_4:hover .Card_Text {
  display: block;
  padding: 0px;
  transition: transform 1s linear 0s;
}


.Card_Image_5:hover .Card_Text {
  display: block;
  transition: transform 1s linear 0s;
}

.Card_Image_5:hover .Card_1_Content {
  height: 280px;
}

@media only screen and (min-width: 680px) and (max-width: 1300px) {
  .Main_tasks_content {
    width: 600px;
    height: auto;
  }

  .Main_tasks_Card {
    flex-wrap: wrap;
    justify-content: center;
  }

  .Card_1 {
    width: 587px;
    height: 287px;
  }

  .Card_Image_1 {
    width: 587px;
    height: 287px;
    padding: 40px 0;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

  .Card_2 {
    width: 587px;
    height: 287px;
    margin-left: 0px;
    display: flex;
    justify-content: space-between;
    margin-top: 15px;
  }

  .Card_Image_2 {
    width: 287px;
    height: 287px;
    padding: 10px 0;
  }

  .Card_Image_3 {
    width: 287px;
    height: 287px;
    margin-left: 0;
    padding: 10px 0;

  }

  .Card_Image_4 {
    margin-top: 0px;
    width: 287px;
    height: 287px;
  }

  .Card_Image_5 {
    margin-top: 0px;
    width: 287px;
    height: 287px;
  }

  .Card_Image_3:hover .Card_1_Content {
    height: 280px;
    display: flex;
    flex-wrap: nowrap;
    margin-left: 20px;

  }

  .Card_Image_3:hover .Card3_Content {
    width: 420px;
    height: 250px;
    display: flex;
    flex-wrap: wrap;
    margin-left: 20px;
    align-items: self-start;
  }

  .Card_Image_3:hover .Card_Title {
    width: auto;
    height: 24px;
    line-height: 24px;
    margin-top: 20px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_3:hover .Card_Text {
    display: block;
    padding: 0px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_3:hover .Card_Image_Icon1 {
    width: 100%;
    height: 40px;
    margin-top: 0px;
    transition: all 1s ease;
  }

  .Card_Image_3:hover .Card_1_Content {
    height: 280px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-left: 0;
    padding: 0px 0px;

  }

  .Card_Image_3:hover .Card3_Content {
    width: 420px;
    height: 250px;
    display: block;
    margin-left: 0px;
    padding: 0 20px;
  }

  .Card_Image_3:hover .Card_Title {
    width: auto;
    height: 24px;
    line-height: 24px;
    margin-top: 20px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_3:hover .Card_Text {
    display: block;
    padding: 0px;
    transition: transform 1s linear 0s;
  }




  .Card_Image_4:hover .Card_Image_Icon1 {
    width: 100%;
    height: 40px;
    margin-top: 0px;
    transition: all 1s ease;
  }

  .Card_Image_4:hover .Card_1_Content {
    height: 280px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-left: 0;
    padding: 0px 0px;

  }

  .Card_Image_4:hover .Card3_Content {
    width: 420px;
    height: 250px;
    display: block;
    margin-left: 0px;
    padding: 0 20px;
  }

  .Card_Image_4:hover .Card_Title {
    width: auto;
    height: 24px;
    line-height: 24px;
    margin-top: 20px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_4:hover .Card_Text {
    display: block;
    padding: 0px;
    transition: transform 1s linear 0s;
  }
}

@media only screen and (min-width: 320px) and (max-width: 679px) {
  .Main_tasks_content {
    padding: 20px;
  }

  .Main_tasks_content {
    width: 287px;
    height: auto;
  }

  .Main_tasks_Card {
    height: auto;
    margin-top: 20px;
    flex-wrap: wrap;
    justify-content: center;
  }

  .Card_1 {
    width: 287px;
    height: 287px;
  }

  .Card_Image_1 {
    width: 287px;
    height: 287px;
    padding: 10px 0;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }

  .Card_2 {
    width: 287px;
    height: auto;
    margin-left: 0px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin-top: 15px;
  }

  .Card_Image_2 {
    width: 287px;
    height: 287px;
    padding: 10px 0;
  }

  .Card_Image_3 {
    width: 287px;
    height: 287px;
    margin-left: 0;
    margin-top: 10px;
    padding: 10px 0;

  }

  .Card_Image_4 {
    margin-top: 0px;
    width: 287px;
    height: 287px;
  }

  .Card_Image_5 {
    margin-top: 10px;
    width: 287px;
    height: 287px;
    margin-left: 0px;
  }

  .Card_Image_3:hover .Card_1_Content {
    height: 280px;
    display: flex;
    flex-wrap: nowrap;
    margin-left: 20px;

  }

  .Card_Image_3:hover .Card3_Content {
    width: 420px;
    height: 250px;
    display: flex;
    flex-wrap: wrap;
    margin-left: 20px;
    align-items: self-start;
  }

  .Card_Image_3:hover .Card_Title {
    width: auto;
    height: 24px;
    line-height: 24px;
    margin-top: 20px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_3:hover .Card_Text {
    display: block;
    padding: 0px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_3:hover .Card_Image_Icon1 {
    width: 100%;
    height: 40px;
    margin-top: 0px;
    transition: all 1s ease;
  }

  .Card_Image_3:hover .Card_1_Content {
    height: 280px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-left: 0;
    padding: 0px 0px;

  }

  .Card_Image_3:hover .Card3_Content {
    width: 420px;
    height: 250px;
    display: block;
    margin-left: 0px;
    padding: 0 20px;
  }

  .Card_Image_3:hover .Card_Title {
    width: auto;
    height: 24px;
    line-height: 24px;
    margin-top: 20px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_3:hover .Card_Text {
    display: block;
    padding: 0px;
    transition: transform 1s linear 0s;
  }




  .Card_Image_4:hover .Card_Image_Icon1 {
    width: 100%;
    height: 40px;
    margin-top: 0px;
    transition: all 1s ease;
  }

  .Card_Image_4:hover .Card_1_Content {
    height: 280px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-left: 0;
    padding: 0px 0px;

  }

  .Card_Image_4:hover .Card3_Content {
    width: 420px;
    height: 250px;
    display: block;
    margin-left: 0px;
    padding: 0 20px;
  }

  .Card_Image_4:hover .Card_Title {
    width: auto;
    height: 24px;
    line-height: 24px;
    margin-top: 20px;
    transition: transform 1s linear 0s;
  }

  .Card_Image_4:hover .Card_Text {
    display: block;
    padding: 0px;
    transition: transform 1s linear 0s;
  }
}</style>