<template >
  <div class="industry_area_Main">
    <div class="industry_area_Main_Content">
      <div class="industry_area_Main_title">
        業種領域
      </div>
      <div class="industry_area_Main_tabs">
        <div class="Tabs_item" :class="{'Tabs_item_active animate__animated animate__fadeIn':active==index}" @click="Tabs_click(index)" v-for="(item, index) in tabs" :key="index">
          <div class="Tabs_item_Content " :class="{'Tabs_item_Content_active animate__animated animate__fadeIn':active==index}">
            <div class="Tabs_item_image">
              <img :src="item.image_scr" alt="">
            </div>
            <div class="Tabs_item_Content_Main">
              <div class="Tabs_item_Content_title">{{item.title}}</div>
              <div class="Tabs_item_Content_main">{{item.content}}</div>
            </div>
          </div>
        </div>
        <div class="Tabs_Btn">
            <div class="Btn_1" @click="Previous"><img src="~/assets/index_image/Previous.png" alt=""></div>
            <div class="Btn_1" @click="Next"><img src="~/assets/index_image/Next.png" alt=""></div>
        </div>
      </div>
    </div>
    <div class="Tabs_ConTent_Div">
      <div class="Tabs_ConTent_Div_Main Tabs_1 animate__animated animate__fadeIn" v-show="active==0">
        <div class="Tabs_ConTent_Div_1_Content">
          <div class="Tabs_ConTent_Div_Content_image">
            <img src="~/assets/index_image/icon_jinrong_white.png" alt="">
            <div class="Tabs_ConTent_Div_Content_title">金融</div>
          </div>
          <div class="Tabs_ConTent_Div_Content_text">
            <div class="Tabs_ConTent_Content_text_1">主な業務経験は製造、流通関係です。</div>
            <div class="Tabs_ConTent_Content_text_2">製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</div>
            <div class="Tabs_ConTent_Content_text_3">システムの最適な開発を行なえる様努力すると伴に、高品質、高性能ソフトウェアプロダクトを提供出来る事を目指しています。</div>
          </div>
        </div>
      </div>
      <div class="Tabs_ConTent_Div_Main Tabs_2 animate__animated animate__fadeIn" v-show="active==1">
        <div class="Tabs_ConTent_Div_1_Content">
          <div class="Tabs_ConTent_Div_Content_image">
            <img src="~/assets/index_image/icon_jinrong_white.png" alt="">
            <div class="Tabs_ConTent_Div_Content_title">金融</div>
          </div>
          <div class="Tabs_ConTent_Div_Content_text">
            <div class="Tabs_ConTent_Content_text_1">主な業務経験は製造、流通関係です。</div>
            <div class="Tabs_ConTent_Content_text_2">製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</div>
            <div class="Tabs_ConTent_Content_text_3">システムの最適な開発を行なえる様努力すると伴に、高品質、高性能ソフトウェアプロダクトを提供出来る事を目指しています。</div>
          </div>
        </div>
      </div>
      <div class="Tabs_ConTent_Div_Main Tabs_3 animate__animated animate__fadeIn" v-show="active==2">
        <div class="Tabs_ConTent_Div_1_Content">
          <div class="Tabs_ConTent_Div_Content_image">
            <img src="~/assets/index_image/icon_jinrong_white.png" alt="">
            <div class="Tabs_ConTent_Div_Content_title">金融</div>
          </div>
          <div class="Tabs_ConTent_Div_Content_text">
            <div class="Tabs_ConTent_Content_text_1">主な業務経験は製造、流通関係です。</div>
            <div class="Tabs_ConTent_Content_text_2">製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</div>
            <div class="Tabs_ConTent_Content_text_3">システムの最適な開発を行なえる様努力すると伴に、高品質、高性能ソフトウェアプロダクトを提供出来る事を目指しています。</div>
          </div>
        </div>
      </div>
      <div class="Tabs_ConTent_Div_Main Tabs_4 animate__animated animate__fadeIn" v-show="active==3">
        <div class="Tabs_ConTent_Div_1_Content">
          <div class="Tabs_ConTent_Div_Content_image">
            <img src="~/assets/index_image/icon_jinrong_white.png" alt="">
            <div class="Tabs_ConTent_Div_Content_title">金融</div>
          </div>
          <div class="Tabs_ConTent_Div_Content_text">
            <div class="Tabs_ConTent_Content_text_1">主な業務経験は製造、流通関係です。</div>
            <div class="Tabs_ConTent_Content_text_2">製造業、物流サービス、通信のソフトウェア開発を得意分野としております。</div>
            <div class="Tabs_ConTent_Content_text_3">システムの最適な開発を行なえる様努力すると伴に、高品質、高性能ソフトウェアプロダクトを提供出来る事を目指しています。</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>

import icon_jinrong from '~/assets/index_image/icon_jinrong.png';
import icon_zhengfu from '~/assets/index_image/icon_zhengfu.png';
import icon_yiliao from '~/assets/index_image/icon_yiliaobaojianyewu-01.png';
import icon_zhizaoye from '~/assets/index_image/icon_zhizaoye.png';
export default {
  data() {
    return {
      active:0,
      tabs:[
        {title:"金融",content:"FINANCE",image_scr:icon_jinrong},
        {title:"政府",content:"GOVERNMENT",image_scr:icon_zhengfu},
        {title:"医療",content:" MEDICAL TREATMENT",image_scr:icon_yiliao},
        {title:"製造業",content:"MANUFACTURE",image_scr:icon_zhizaoye},
      ]
    }
  },
  methods:{
    Tabs_click(index){
      this.active=index
    },
    Previous(){
      if(this.active==0){
        this.active=3
      }
      else{
        this.active-=1
      }
    },
    Next(){
      if(this.active==3){
        this.active=0
      }
      else{
        this.active+=1
      }
    }
  }
}
</script>
<style >
.industry_area_Main {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  transform: translateY(-340px);
}

.industry_area_Main_Content {
  width: 1200px;
  margin-top: 120px;

}

.industry_area_Main_title {
  height: 36px;
  font-size: 36px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 36px;
}

.industry_area_Main_tabs {
  margin-top: 80px;
  height: 104px;
  display: flex;
  flex-wrap: nowrap;
}
.Tabs_item{
  width: 250px;
  height: 104px;
  background: #0E1B47;
  color: #FFFFFF;

}
.Tabs_item_active{
  background: rgba(255, 255, 255, 0.06);
}
.Tabs_item_Content{
  width: 100%;
  height: 100%;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #597BE5;
  line-height: 30px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.Tabs_item_Content_active{
  border-top: 4px solid #597ce5;
}
.Tabs_item_image{
  width: 40px;
  height: 40px;
}
.Tabs_item_Content_Main{
  height: 40px;
  margin-left: 14px;
}
.Tabs_item_Content_title{
  height: 23px;
  font-size: 24px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #597BE5;
  line-height: 23px;
}
.Tabs_item_Content_main{
  height: 9px;
  margin-top: 10px;
  font-size: 12px;
  font-family: Roboto;
  font-weight: 500;
  color: #597BE5;
  line-height: 9px;
}
.Tabs_ConTent_Div{
  width: 100%;
  height: 580px;
}
.Tabs_ConTent_Div_Main{
  width: 100%;
  height: 580px;
  display: flex;
  justify-content: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.Tabs_1{
  background-image: url('~/assets/index_image/pic_jinrong.png');
}
.Tabs_2{
  background-image: url('~/assets/index_image/pic_zhengfu.png');
}
.Tabs_3{
  background-image: url('~/assets/index_image/pic_yiliao.png');
}
.Tabs_4{
  background-image: url('~/assets/index_image/pic_zhizaoye.png');
}
.Tabs_ConTent_Div_1_Content{
  width: 1200px;
  height: 580px;
  padding: 0 45px;

}
.Tabs_ConTent_Div_Content_image{
  width: 100%;
  height: 40px;
  display: flex;
  flex-wrap: wrap;
  margin-top: 100px;
}
.Tabs_ConTent_Div_Content_image img{
  width: 40px;
  height: 40px;
}
.Tabs_ConTent_Div_Content_title{
  height: 33px;
  font-size: 36px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 30px;
  margin-left: 14px;
}
.Tabs_ConTent_Div_Content_text{
  width: 100%;
  margin-top: 60px;
  margin-left: 60px;
  font-size: 16px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 24px;
}
.Tabs_ConTent_Content_text_2{
  margin-top: 1rem;
}
.Tabs_Btn{
  width: 130px;
  height: 104px;
  margin-left: 70px;
  display: flex;
  align-items: center;
}
.Btn_1{
  width: 64px;
  height: 64px;
  border: 1px solid #5A7BE5;
  display: flex;
  justify-content: center;
  align-items: center;
}
@media only screen and (min-width: 1300px) and (max-width: 1440px) {
  .industry_area_Main{
    transform: translateY(0px);
  }
}
@media only screen and (min-width: 1024px) and (max-width: 1300px) {
  .industry_area_Main{
    transform: translateY(0px);
  }
  .industry_area_Main_Content{
    width: 900px;
  }
  .Tabs_ConTent_Div_1_Content{
    width: 900px;
  }
  .industry_area_Main_tabs{
    height: 115px;
  }
  .Tabs_item{
    height: 115px;
  }
  .Tabs_item_Content{
    display: block;
    padding: 7.5px 0;
  }
  .Tabs_item_image{
    width: 100%;
    display: flex;
    justify-content: center;
  }
  .Tabs_item_Content_Main{
    margin-left: 0;
    text-align: center;
    margin-top: 10px;
  }
}
@media only screen and (min-width: 320px) and (max-width: 1023px) {
  .industry_area_Main{
    transform: translateY(0px);
  }
}
</style>