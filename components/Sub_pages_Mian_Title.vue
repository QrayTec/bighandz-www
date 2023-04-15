<template>
  <div class="Sub_pages_Mian_Title">
    <div class="Sub_pages_Mian_Title_Content">
      <div class="Main_Title_Content">
        <div  class="Main_Title_1">
          <RouteBreadcrumbs class="RouteBreadcrumbs_Bar"></RouteBreadcrumbs>
          <div class="Sub_pages_Title">
            <div class="Mian_Big_title">
              {{Main_title}}
            </div>
            <div class="Mian_Min_title">{{Min_title}}</div>
            <div class="Border_Line"></div>
          </div>
        </div>
        <div class="Sub_pages_Iamge">
          <div class="Sub_pages_Iamge_Content">
            <img :src="image" alt="">
          </div>

        </div>
      </div>
    <div class="Sub_pages_Iamge_Line"></div>
    </div>

  </div>
</template>
<script>
export default {
  props:{
    Main_title:{
      type: String,
      required: true,
    },
    Min_title:{
      type: String,
      required: true,
    },
    image:{
      type: String,
      required: true,
      // 父组件要写setup
    }
  },

}
</script>
<style>
  .Sub_pages_Mian_Title{
    width: 100%;
    height: 600px;
    background-color: rgba(14, 27, 71, 1);
    display: flex;
    justify-content: center;
  }
  .Sub_pages_Mian_Title_Content{
    position: relative;

    width: 1536px;
    padding-top: 80px;
    padding-left: 168px;
  }
  .Main_Title_Content{
    width: 100%;
    margin-top: 80px;
    display: flex;
    flex-wrap: wrap;
  }
  .Main_Title_1{
    width: 50%;
    display: flex;
    flex-direction: column;
  }
  .RouteBreadcrumbs_Bar{
    width: 100%;
  }
  .Sub_pages_Title{
    margin-top: 120px;
    display: flex;
    flex-direction: column;
  }
  .Mian_Big_title{
    font-size: 56px;
    font-family: Noto Sans JP;
    font-weight: normal;
    color: #FFFFFF;
    line-height: 56px;
  }
  .Mian_Min_title{
    margin-top: 20px;
    height: 15px;
    font-size: 18px;
    font-family: Roboto;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 15px;
    opacity: 0.4;
    letter-spacing: 0.9rem;
    text-transform: uppercase;
  }
  .Border_Line{
    margin-top: 40px;
    width: 60px;
    height: 8px;
    background-color: rgba(103, 133, 193, 1);
  }
  .Sub_pages_Iamge{
    width: 50%;
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }
  .Sub_pages_Iamge_Content{
    width: 390px;
    height: 390px;
  }
  .Sub_pages_Iamge_Line{
    width: 379px;
    height: 37px;
    background: #6785C1;
    position: absolute;
    bottom: 10.5%;
    right: -6.8%;
  }
  @media only screen and (min-width: 1300px) and (max-width: 1760px) {
    .Sub_pages_Mian_Title_Content{
      width: 1100px;
      padding-left: 0;

    }
    .Mian_Min_title{
      letter-spacing:1rem;
    }
  }
  @media only screen and (min-width: 768px) and (max-width: 1299px) {
    .Sub_pages_Mian_Title_Content{
      width: 600px;
      padding-left: 0;

    }
    .Mian_Big_title{
      font-size: 40px;
    }
    .Mian_Min_title{
      letter-spacing:0.2rem;
    }
    .Sub_pages_Iamge_Line{
      bottom: 23%;
      right: -10%;
    }
    .Sub_pages_Iamge_Line{
      width:250px;
      bottom: 30%;
    }
    .Sub_pages_Title{
      margin-top: 60px;
    }
  }
  @media only screen and (max-width: 767px) {
    .Sub_pages_Mian_Title{
      height: auto;
    }
    .Sub_pages_Mian_Title_Content{
      width: 80%;
      padding-left: 0;
    }
    .Main_Title_1{
      width: 100%;
    }
    .Sub_pages_Title{
      margin-top: 20px;
    }
    .Sub_pages_Iamge{
      margin-top: 60px;
      width: 100%;
      justify-content: center;
    }
    .Mian_Big_title{
      font-size: 36px;
    }
    .Mian_Min_title{
      font-size: 18px;
      letter-spacing:0.15rem;
    }
    .Sub_pages_Iamge_Line{
      width:70%;
    }
    .Main_Title_Content{
      margin-top: 20px;
      margin-bottom: 40px;
    }
    .Border_Line{
      margin-top: 20px;
    }
    .Sub_pages_Iamge_Content{
      width: 100%;
      height: auto;
      display: flex;
      justify-content: center;
    }
  }
</style>