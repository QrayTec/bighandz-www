<template>
  <div class="Related_Company">
    <header>
      <HeaderNavBar :active_props=1></HeaderNavBar>
    </header>
    <main>
      <section>
        <div class="First_main">
          <SubPagesMianTitle Main_title="関連 · 会社" Min_title="Associated company" :image="pic_guanlianhuishe">
          </SubPagesMianTitle>
        </div>
      </section>
      <section>
        <div class="Related_Company_Main">
         <div class="Related_Company_Section">
          <div class="Related_Company_Section_Main" :class="{'m_t_120':index!=0}" v-for="(item, index) in Company_Info" :key="index">
            <div class="Company_Image" :class="index!=0?'order_1':'order_0'" >
              <img :src=item.Image_src alt="">
            </div>
            <div class="Company_Info" :class="index%2==0?'p_l_20':'p_r_20'">
              <div class="Company_Info_title">{{item.Company_Name}}</div>
              <div class="Company_Info_hr"></div>
              <div class="Company_Info_hr_2"></div>
              <div class="Company_Info_main m_t_20" v-show="Company_Info_main_index!=4||index==1"  v-for="(item, Company_Info_main_index) in Company_Info_main" :key="Company_Info_main_index">
                  <div class="Company_Info_main_left">
                    <img src="" alt="">
                    <div class="Company_Info_main_title">{{item.info_title}}</div>
                  </div>
                  <div class="Company_Info_main_Content" v-if="Company_Info_main_index!=4">{{index==0?item.info_Content:item.info_Content_2}}</div>
                  <div class="Company_Info_main_Content" v-if="Company_Info_main_index==4"><a :href="item.info_Content_2" target="_blank">{{item.info_Content_2}}</a></div>
              </div>
            </div>
          </div>
         </div>
        </div>
      </section>
    </main>
    <footer>
      <Footer></Footer>
    </footer>
  </div>
</template>
<script>
import pic_guanlianhuishe from '~/assets/Aubot_us/pic_guanlianhuishe.png';
import pic_qingdao from '~/assets/Aubot_us/pic_qingdao.png';
export default {
  data() {
    return {
      Company_Info:[
        {Image_src:"",Company_Name:"北京大手計算機技術有限公司"},
        {Image_src:pic_qingdao,Company_Name:"青島大手海恩信息技術有限公司"},
      ],
      Company_Info_main:[
        {info_Icon:"", info_title:"住所",info_Content:"北京市東城区広渠家園冠城名敦道4号楼10層",info_Content_2:"山東省青島市高新区秀園路2号科創慧谷D2-4",},
        {info_Icon:"", info_title:"社員数",info_Content:"60名",info_Content_2:"200名",},
        {info_Icon:"", info_title:"TEL",info_Content:"86-10-6823-0715",info_Content_2:"86-0532-68012198",},
        {info_Icon:"", info_title:"FAX",info_Content:"86-10-6823-0714",info_Content_2:"86-0532-68012123",},
        {info_Icon:"", info_title:"主页",info_Content:"",info_Content_2:"http://www.qdhaien.cn/",}
      ]
    }
  },
  setup(){
    return {pic_guanlianhuishe,}
  },
  mounted() {
    if (process.client) {
      document.title = '企業情報 - 関連 · 会社'
    }
  }
}
</script>
<style>
  .p_l_20{
    padding-left: 20px;
  }
  .p_r_20{
    padding-right: 20px;
  }
  .m_t_20{
    margin-top: 20px;
  }
  .m_t_38{
    margin-top: 38px;
  }
  .m_t_120{
    margin-top: 120px;
  }
  .order_0{
    order: 0;
  }
  .order_1{
    order: 1;
  }
  .Related_Company_Main{
    width: 100%;
    display: flex;
    justify-content: center;
  }
  .Related_Company_Section{
    width: 1200px;
    padding: 120px 0;
  }
  .Related_Company_Section_Main{
    display: flex;
  }
  .Company_Image{
    width: 40%;
    display: flex;
    justify-content: center;
  }
  .Company_Info{
    width: 60%;
  }
  .Company_Image img{
    width: 488px;
    height: 325px;
    background: #6785C1;
  }
  .Company_Info_title{
    font-size: 36px;
    font-family: Noto Sans JP;
    font-weight: bold;
    color: #070F26;
  }
  .Company_Info_hr{
    width: 100%;
    height: 2px;
    background: #6785C1;
    margin-top: 18px;
  }
  .Company_Info_hr_2{
    width: 100%;
    height: 1px;
    margin-top: 4px;
    background-image: linear-gradient(to right, #6785C1 0%, #6785C1 50%, transparent 50%);
    background-size: 8px 1px;
    background-repeat: repeat-x;
  }
  .Company_Info_main{
    padding: 0  20px;
    display: flex;
  }
  .Company_Info_main_left{
    display: flex;
    align-items: center;
  }
  .Company_Info_main_left img{
    width: 14px;
    height: 14px;
    background-color: black;
  }

  .Company_Info_main_title{
    width: 48px;
    font-size: 16px;
    font-family: Noto Sans JP;
    font-weight: bold;
    color: #070F26;
    margin-left: 10px;
  }
  .Company_Info_main_Content{
    font-size: 16px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #070F26;
    margin-left: 54px;
  }
  @media only screen and (min-width: 768px) and (max-width: 1299px){
    .Related_Company_Section{
      width: 80%;
    }
    .Company_Image{
      min-width: 325px;
      min-height: 325px;
      align-items: center;
    }
  }
  @media only screen and (max-width: 767px){
    .Related_Company_Section{
      width: 80%;
    }
    .Related_Company_Section_Main{
      flex-wrap: wrap;
    }
    .Company_Image{
      width: 100%;
    }
    .Company_Info{
      width: 100%;
      margin-top: 20px;
    }
    .Company_Info_main_left img{
      width: 14px;
      height: 14px;
      background-color: black;
      object-fit: cover;
    }
    .Company_Info_main{
      flex-wrap: wrap;
      justify-content: space-between;
    }
    .Company_Info_main_Content{
      margin-left: 0;
    }
    .Company_Image{
      margin-top: 20px;
    }
    .Company_Image img{
      width: 300px;
      height: 300px;
    }
    .m_t_120{
      margin-top: 60px;
    }
    .p_l_20{
      padding-left: 0;
    }
    .p_r_20{
      padding-right: 0;
    }
  }
</style>