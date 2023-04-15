<template>
  <div class="About_US">
    <header>
      <HeaderNavBar :active_props=1></HeaderNavBar>
    </header>
    <main>
      <div class="First_main">
        <SubPagesMianTitle 
        Main_title="社長 · からのメッセージ" 
        Min_title="Message from the President" 
        :image="jingyinglinian">
      </SubPagesMianTitle>
      </div>
    </main>
    <footer>
      <Footer></Footer>
    </footer>
  </div>
</template>
<script>
import jingyinglinian from '~/assets/Aubot_us/pic_message_banner.png';
export default  {
  data() {
    return {
      active: this.$route.params.active,
    }
  },
  setup(){
    return{
      jingyinglinian,
    }
  },
  mounted(){
    if (process.client) {
        document.title = '企業情報-経営理念'
      }
  }
}

</script>
<style ></style>