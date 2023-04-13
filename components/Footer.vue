<template>
  <div class="Footer">
    <div class="Footer_Main">
      <div class="Footer_logo">
        <img src="~/assets/index_image/BigHandzCo.Ltd.png" alt="">
      </div>
      <div class="Footer_List_Content">
        <div class="List_data" v-for="(item, index) in Footer_List_Content" :key="index">
          <div class="Footer_Line"></div>
        <div class="Footer_List_Text">{{item.Content}}</div>
        <div class="Footer_Line"></div>
        </div>
      </div>
      <div class="Footer_Copyright">
        Copyright © BigHandz Co.Ltd. All Rights Reserved.
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      Footer_List_Content:[
        {Content:"ホーム"},
        {Content:"個人情報保護方針"},
        {Content:"利用規約"},
        {Content:"お問い合わせ"},
      ]
    }
  },
}
</script>
<style>
  .Footer{
    width: 100%;
    height: 150px;
    background: #09122E;
    display: flex;
    justify-content: center;
  }
  .Footer_Main{
    width: 1200px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    color: #FFFFFF;
  }
  .Footer_Line{
    width: 1px;
    height: 12px;
    background-color: rgba(255, 255, 255, 0.2);
  }
  .Footer_List_Content{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .List_data{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .Footer_List_Text{
    height: 12px;
    font-size: 15px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 12px;
    margin: 0px 20px ;
  }
  @media only screen and (min-width: 768px) and (max-width: 1300px) {
    .Footer_Main{
      width: 600px;
      flex-wrap:wrap;
    }
    .Footer_logo{
      width: 100%;
      display: flex;
      justify-content: center;
      margin-top: 10px;

    }
    .Footer_List_Content{
      width: 100%;
      margin-top: 10px;
    }
    .Footer_Copyright{
      width: 100%;
      display: flex;
      justify-content: center;
      margin-top: 10px;
    }
  }
  @media only screen and (max-width: 768px){
    .Footer{
      height: auto;
    }
    .Footer_Main{
      width: 300px;
      height: auto;
      flex-wrap:wrap;
    }
    .Footer_logo{
      width: 100%;
      display: flex;
      justify-content: center;
      margin-top: 10px;

    }
    .Footer_List_Content{
      width: 100%;
      margin-top: 10px;
      display: flex;
      flex-wrap: wrap;
    }
    .Footer_List_Text{
      width: 140px;
      margin: 0px;
      text-align: center;
    }
    .List_data{
      margin-top: 10px;
    }
    .Footer_Copyright{
      text-align: center;
      margin-top: 10px;
    }
  }
</style>