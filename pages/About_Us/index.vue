<template>
  <div class="About_US">
    <header>
      <HeaderNavBar :active_props=1></HeaderNavBar>
    </header>
    <main>
      <div class="First_main">
        <SubPagesMianTitle Main_title="経営·理念" Min_title="Business philosophy" :image="jingyinglinian">
        </SubPagesMianTitle>
      </div>
      <div class="About_US_Main">
        <div class="About_US_Main_Content">
          <div class="About_US_Main_Image">
            <img src="~/assets/Aubot_us/pic_jingyinglinian.png" alt="pic_jingyinglinian">
          </div>
          <div class="About_US_Main_Text">
            <div class="About_US_Main_Text_Main">
              <span>株式会社ビッグハンズ</span>
              は中国の優秀な人材と、日本の高度な技術・ノウハウを融合し、日中を中心としたSI事業・ITソリューション事業を展開して行きます。<br>
              日中を完全に結合させた中国発のSI事業者の リーディングカンパニーとしての地位を維持しつつ、 国、人種の垣根を超えた、広い社会貢献を標榜(ひょうぼう)致します。
            </div>
            <div class="About_US_Main_Text_Min">
              <div class="About_US_Min_Text">経営·理念</div>
              <div class="About_US_Min_Text_En">Business philosophy</div>
              <div class="About_US_Min_Line"></div>
            </div>
          </div>
        </div>
      </div>
    </main>
    <footer>
      <Footer></Footer>
    </footer>
  </div>
</template>
<script>
import jingyinglinian from '~/assets/Aubot_us/pic_jingyinglinian_banner.png';
export default {
  data() {
    return {
      active: this.$route.params.active,
    }
  },
  setup() {
    return {
      jingyinglinian,
    }
  },
  mounted() {
    if (process.client) {
      document.title = '企業情報-経営理念'
    }
  }
}

</script>
<style>
.About_US_Main{
  width: 100%;
  height: 700px;
  padding: 120px 0;
  display: flex;
  justify-content: center;
}
.About_US_Main_Content{
  width: 1200px;
  display: flex;
}
.About_US_Main_Image{
  width: 57.5%;
}
.About_US_Main_Text{
  width: 42.5%;
  padding: 20px 0px 20px 20px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.About_US_Main_Text_Main{
  font-size: 16px;
  font-family: Noto Sans JP;
  color: #070F26;
  font-weight: 500;
}
.About_US_Main_Text_Main span{
  font-weight: bold;
}
.About_US_Main_Text_Min{
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-direction: column;
}
.About_US_Min_Text{
  height: 24px;
  font-size: 24px;
  font-family: Noto Sans JP;
  font-weight: bold;
  color: #070F26;
  line-height: 15px;
}
.About_US_Min_Text_En{
  margin-top: 10px;
  height: 15px;
  font-size: 12px;
  font-family: Roboto;
  font-weight: 400;
  color: #070F26;
  line-height: 15px;
  opacity: 0.4;
  text-transform: uppercase;
}
.About_US_Min_Line{
  margin-top: 10px;
  width: 40px;
  height: 5px;
  background: #6785C1;
}
@media only screen and (min-width: 768px) and (max-width: 1299px) {
  .About_US_Main{
    height: auto;
    padding: 60px 0;
  }
  .About_US_Main_Content{
    width: 600px;
    flex-wrap: wrap;
  }
  .About_US_Main_Image{
    width: 100%;
  }
  .About_US_Main_Text{
    margin-top: 40px;
    padding: 0;
    width: 100%;
  }  
  .About_US_Main_Text_Min{
    margin-top: 40px;
  }
}
@media only screen  and (max-width:767px) {
  .About_US_Main{
    padding: 60px 0;
    height: auto;
  }
  .About_US_Main_Content{
    width: 80%;
    flex-wrap: wrap;
  }
  .About_US_Main_Image{
    width: 100%;
  }
  .About_US_Main_Text{
    margin-top: 40px;
    padding: 0;
    width: 100%;
  }
  .About_US_Main_Text_Min{
    margin-top: 40px;
  }
}
</style>