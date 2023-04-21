<template>
  <div class="MaJor_Clients">
    <div class="Major_Clients_Main">
      <div class="Major_Clients_Content">
        <div class="MaJor_Clients_title">
          主要顧客
        </div>
      <div class="MaJor_Clients_List" >
        <div class="Main_List" v-for="(item, index) in MaJor_Clients_List" :key="index">
          <div class="MaJor_Clients_Iamge">
            <img :src="item.image_src" alt="">
          </div>
        </div>
      </div>
      </div>
    </div>
  </div>
</template>
<script>
import Nce from '~/assets/index_image/NCE_logo.png';
import Nri from '~/assets/index_image/NRI_logo.png';
import Ncr from '~/assets/index_image/NCR_logo.png';
import Nec from '~/assets/index_image/NEC_logo.png';
import Ydc from '~/assets/index_image/YDC_logo.png';
import Astellas from '~/assets/index_image/Astellas_logo.png';
export default {
  data() {
    return {
      MaJor_Clients_List:[
        {image_src:Nce},
        {image_src:Nec},

        {image_src:Nri},
        {image_src:Ydc},

        {image_src:Ncr},
        {image_src:Astellas},
      ]
    }
  },
}
</script>
<style>
  .MaJor_Clients{
    margin-top: 580px;
    height: 840px;
    background-position:center;
    background-repeat: no-repeat;
    background-size: cover;
    background-color: transparent;
  }
  .Major_Clients_Main{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    background: linear-gradient(0deg, #0E1B47, rgba(14,27,71,0.25));
  }
  .Major_Clients_Content{
    width: 1200px;
    height: auto;
    padding: 120px 0px;
  }
  .MaJor_Clients_title{
    width: auto;
    height: 36px;
    font-size: 36px;
    font-family: Noto Sans JP;
    font-weight: 500;
    color: #FFFFFF;
    line-height: 36px;
  }
  .MaJor_Clients_List{
    margin-top: 80px;
    width: 100%;
    height: 300px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    flex-direction: column;

  }
  .Main_List{
    width: 387px;
    height: 120px;
    background: rgba(9,18,46,0.2);
    border: 1px solid rgba(255,255,255,0.08);

  }
  .MaJor_Clients_Iamge{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  @media only screen and (min-width: 1300px) and (max-width: 1440px) {
    .MaJor_Clients{
      margin-top: 0px;
    }
  }
  @media only screen and (min-width: 1024px) and (max-width: 1300px) {
    .MaJor_Clients{
      margin-top: 0px;
    }
    .Major_Clients_Content{
      width: 900px;
      padding: 120px 0px;
    }
    .MaJor_Clients_List{
      height: auto;
      flex-direction:row;
    }
    .Main_List{
      margin-top: 20px;
    }
  }
  @media only screen and (min-width: 768px) and (max-width: 1023px) {
    .MaJor_Clients{
      margin-top: 0px;
    }
    .Major_Clients_Content{
      width: 600px;
      padding: 120px 0px;
    }
    .MaJor_Clients_List{
      height: auto;
      flex-direction:row;
    }
    .Main_List{
      width: 280px;
      margin-top: 20px;
    }
  }
  @media only screen and (max-width: 767px) {
    .MaJor_Clients{
      height: auto;
      margin-top: 0px;
    }
    .Major_Clients_Content{
      width: 300px;
      padding: 120px 0px;
    }
    .MaJor_Clients_List{
      height: auto;
      flex-direction:row;
    }
    .Main_List{
      width: 280px;
      margin-top: 20px;
    }
  }
</style>