<template>
  <div class="Company_Introduction_Development_Process">
    <header>
      <HeaderNavBar :active_props=1></HeaderNavBar>
    </header>
    <main>
      <section>
        <div class="First_main">
          <SubPagesMianTitle Main_title="会社概要と沿革" Min_title="Company Introduction and Development Process" :image="pic_Company_Profile_History">
          </SubPagesMianTitle>
        </div>
      </section>
      <section>
        <div class="Company_Introduction_Development_Process_Main">
12
        </div>
      </section>
    </main>
  </div>
</template>
<script>
import pic_Company_Profile_History from '~/assets/Aubot_us/pic_Company_Profile_History.png';

export default {
  setup(){
    return {pic_Company_Profile_History,}
  }
}
</script>
<style>
  
</style>