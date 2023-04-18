<template>
  <div class="About_US">
    <header>
      <HeaderNavBar :active_props=1></HeaderNavBar>
    </header>
    <main>
      <section>
        <div class="First_main">
          <SubPagesMianTitle Main_title="社長 · からのメッセージ" Min_title="Message from the President" :image="jingyinglinian">
          </SubPagesMianTitle>
        </div>
      </section>
      <section>
        <div class="Message_President">
          <div class="Message_President_Content">
            <div class="Message_President_Content_Text">
              <div class="Message_President_Content_Title">
                中国と日本の橋渡し役に!
              </div>
              <div class="Message_Content" :class="{'m_top_2rem':index!=0}" v-for="(item, index) in Message_Content" :key="index">
              {{ item.context }}
              </div>
              <div class="President_Content">社长からのメッセージ</div>
            </div>
            <div class="Message_President_Content_Image">
              <div class="President_Image"></div>
              <div class="President_Context">代表取締役</div>
              <div class="President_Image2"><img src="~/assets/Aubot_us/pic_shezhangqianming.png" alt=""></div>
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
import jingyinglinian from '~/assets/Aubot_us/pic_message_banner.png';
export default {
  data() {
    return {
      active: this.$route.params.active,
      Message_Content:[
       { context:"当社は『中国と日本の橋渡し役に』をスローガンに日中の情報システム開発に奉仕するため、１９９８年に設立されました。"},
       { context:"以来、アプリケーション、ソフトパッケージの提供、各種受託業務等の情報関連事業を進めてまいりました。"},
       { context:"２００２年９月から北京ビッグハンズでは日本企業からのシステム開発の業務を積極的に行い R&D の役割を果たすオフショア開発のビジネスモデルを確立し、高品質な成果物を提供してまいりました。今後日本と中国をビジネスの舞台として、更なるサービス を提供するトータル・システム・プロバイダーとして誠心誠意で行っていく所存で御座います。"},
       { context:"私達が企業を経営する上で考えていることは、中国的な経営の良い部分と、日本的な経営の良い部分をきっちりと融合させ、新しい経営スタイルを作り出していくことです。"},
       { context:"日本での経営経験と中国経営のノウハウや文化・風土を熟知している強みを活用して日本企業が中国に進出する際のコンサルトと IT 面からサポートしていく事業と技術の高い中国人を活用してのオフショア開発事業をさらに拡大しトータル・システム・プロバイダーとして邁進してまいりま す。これらを進めるベースとして単なるコストマネジメントに偏ることなく、『ビジネスは共に Win － Win でなければならない』と日頃から考えております。"},
      ]
    }
  },
  setup() {
    return {
      jingyinglinian,
    }
  },
  mounted() {
    if (process.client) {
      document.title = '企業情報-社長からのメッセージ'
    }
  }
}

</script>
<style>
.Message_President{
  width: 100%;
  padding: 120px 0;
  display: flex;
  justify-content: center;
}
.Message_President_Content{
  width: 1200px;
  display: flex;
}
.Message_President_Content_Text{
  width:56.25%;
}
.Message_President_Content_Image{
  width: 43.75%;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}
.Message_President_Content_Title{
  font-size: 36px;
  font-family: Noto Sans JP;
  font-weight: bold;
  color: #070F26;
  line-height: 32px;
}
.Message_Content{
  margin-top: 60px;
  font-size: 16px;
  font-family: Noto Sans JP;
  font-weight: 400;
  color: #070F26;
  line-height: 30px;
}
.m_top_2rem{
  margin-top: 2rem;
}
.President_Content{
  margin-top: 60px;
  font-size: 16px;
  font-family: Noto Sans JP;
  font-weight: 400;
  color: #070F26;
  line-height: 16px;
}
.President_Image{
  width: 480px;
  height: 600px;
  background: #5F7DDE;
}
.President_Context{

  margin-top: 30px;
}
.President_Image2{
  width: 240px;
  height: 80px;
  margin-top: 20px;
}
@media only screen and (min-width: 768px) and (max-width: 1299px) {
  .Message_President_Content{
    width: 80%;
    flex-wrap: wrap;
  }
  .Message_President_Content_Text{
    width:100%;
  }
  .Message_President_Content_Image{
    margin-top: 60px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
}
@media only screen  and (max-width:767px) {
  .Message_President_Content{
    width: 80%;
    flex-wrap: wrap;
  }
  .Message_President_Content_Text{
    width:100%;
  }
  .Message_President_Content_Image{
    margin-top: 60px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .President_Image{
    width:100%;
  }
}
</style>