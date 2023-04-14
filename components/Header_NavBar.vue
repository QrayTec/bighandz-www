<template>
  <div class="Nav_Bar" :class="{ 'Nav_Bar_h': NavbarShow }">
    <div class="Nav_Bar_List_data">
      <div class="NavBar_Main">
        <div class="NavBar_Main_List">
          <div class="NavBar_logo">
            <img src="~/assets/index_image/BigHandzCo.Ltd.png" alt="">
          </div>

          <div class="nav_bar_button">
            <button type="button" class="menu_Btn" @click="isShowList()">
              <svg t="1681467975270" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg"
                p-id="2620" width="30" height="30">
                <path
                  d="M133.310936 296.552327l757.206115 0c19.781623 0 35.950949-16.169326 35.950949-35.950949 0-19.781623-15.997312-35.950949-35.950949-35.950949L133.310936 224.650428c-19.781623 0-35.950949 16.169326-35.950949 35.950949C97.359987 280.383 113.529313 296.552327 133.310936 296.552327z"
                  fill="#ffffff" p-id="2621"></path>
                <path
                  d="M890.51705 476.135058 133.310936 476.135058c-19.781623 0-35.950949 16.169326-35.950949 35.950949 0 19.781623 16.169326 35.950949 35.950949 35.950949l757.206115 0c19.781623 0 35.950949-16.169326 35.950949-35.950949C926.467999 492.304384 910.298673 476.135058 890.51705 476.135058z"
                  fill="#ffffff" p-id="2622"></path>
                <path
                  d="M890.51705 727.447673 133.310936 727.447673c-19.781623 0-35.950949 15.997312-35.950949 35.950949s16.169326 35.950949 35.950949 35.950949l757.206115 0c19.781623 0 35.950949-15.997312 35.950949-35.950949S910.298673 727.447673 890.51705 727.447673z"
                  fill="#ffffff" p-id="2623"></path>
              </svg>
              <span class="sr-only">Icon description</span>
            </button>
          </div>
        </div>
        <div class="NavBar_List" v-show="NavbarShow">
          <NuxtLink class="NavBar_List_Content" :to="item.link" v-for="(item, index) in Navbar_Data" :key="index"
            :class="{ 'active_Text': active == index }">
            <div class="NavBar_List_Content " @click="NavBar_click(index)">
              {{ item.title }}
              <div class="active_List" v-show="active == index"></div>
            </div>
          </NuxtLink>
        </div>
      </div>

    </div>
    <div class="Secondary_Menu" v-show="Secondary_Menu_Flag">
      <div class="Secondary_Menu_Data">
        <div class="Secondary_Menu_title">
          <div class="Secondary_Menu_Icon">
            <img src="~/assets/NavBar/icon_gongsixinxi.png" alt="">
          </div>
          <div class="Secondary_Menu_title_Text">企業情報</div>
        </div>
        <div class="Secondary_Menu_List">
          <div class="Secondary_Menu_List_Data" v-for="(item, index) in Secondary_Menu_List_Data" :key="index">
            <nuxt-link :to="item.link">
              {{ item.title }}
            </nuxt-link>
          </div>
        </div>
      </div>

    </div>
    <div class="Secondary_Menu_Close"  v-show="Secondary_Menu_Flag" @click="Secondary_Menu_Close"></div>
  </div>
</template>
<script>
import gongsixinxi from '~/assets/NavBar/icon_gongsixinxi.png';
import yewugaishu from '~/assets/NavBar/icon_yewugaishu.png';
import zhaopinxinxi from '~/assets/NavBar/icon_zhaopinxinxi.png';
export default {
  data() {
    return {
      active: 0,
      Navbar_Data: [
        { title: "ホーム", link: '/' },
        { title: "企業情報", },
        { title: "事業概要", },
        { title: "採用情報", },
        { title: "関連会社", link: '/' },
      ],
      Secondary_Menu_Flag: false,
      Secondary_Menu_List_1: [
        { title: "経営理念", link: '/About_Us' },
        { title: "社長からのメッセージ", link: '/About_Us/' },
        { title: "会社概要と沿革", link: '/' },
        { title: "関連会社", link: '/' },
      ],
      Secondary_Menu_List_2: [
        { title: "システム開発事業", link: '/' },
        { title: "インフラ基盤事業", link: '/' },
        { title: "オフショア事業", link: '/' },
        { title: "コンサルテイング事業", link: '/' },
        { title: "ヘルスケア事業", link: '/' },
        { title: "開発実績", link: '/' },
      ],
      Secondary_Menu_List_3: [
        { title: "新卒採用", link: '/' },
        { title: "キャリア採用", link: '/' },
        { title: "社員より", link: '/' },
      ],
      Secondary_Menu_List_Data: [],
      Secondary_Menu_Title: "企業情報",
      Secondary_Menu_Icon: gongsixinxi,
      NavbarShow: false,
    }
  },
  mounted() {
    this.Secondary_Menu_List_Data = this.Secondary_Menu_List_1;
    window.addEventListener('resize', this.checkScreenSize)
    this.checkScreenSize()
  },
  methods: {
    isShowList() {
      this.NavbarShow = !this.NavbarShow;

    },
    checkScreenSize() {
      if (window.innerWidth < 768) {
        this.NavbarShow = false
      } else {
        this.NavbarShow = true
      }
    },
    NavBar_click(index) {
      this.active = index;
        this.Secondary_Menu_Flag = !this.Secondary_Menu_Flag
      if (index == 1 || index == 2 || index == 3) {
        this.Secondary_Menu_Flag = true
      }
    },
    Secondary_Menu_Close(){
      this.Secondary_Menu_Flag = false
    }
  },
  watch: {
    NavbarShow(newValue, oldValue) {
      if (!newValue) {
        this.Secondary_Menu_Flag = false

      }
    },
    active(newValue, oldValue) {
      if (newValue == 1) {
        this.Secondary_Menu_Title = "企業情報",
          this.Secondary_Menu_Icon = gongsixinxi,
          this.Secondary_Menu_List_Data = this.Secondary_Menu_List_1;
      }
      else if (newValue == 2) {
        this.Secondary_Menu_Title = "事業概要",
          this.Secondary_Menu_Icon = yewugaishu,
          this.Secondary_Menu_List_Data = this.Secondary_Menu_List_2;
      }
      else if (newValue == 3) {
        this.Secondary_Menu_Title = "採用情報",
          this.Secondary_Menu_Icon = zhaopinxinxi,
          this.Secondary_Menu_List_Data = this.Secondary_Menu_List_3;
      }
      else {
        this.Secondary_Menu_Title = "企業情報",
          this.Secondary_Menu_Icon = gongsixinxi,
          this.Secondary_Menu_List_Data = this.Secondary_Menu_List_1;
      }
    }
  }
}
</script>
<style>
.m_top_20 {
  margin-top: 16px;
}
.Secondary_Menu_Close{
  height: 100vh;
}
.Nav_Bar {
  width: 100%;
  height: 80px;
  background-color: #0E1B47;

}

.menu_Btn {
  display: none;
}

.Nav_Bar_List_data {
  width: 100%;
  display: flex;
  justify-content: center;
}

.NavBar_Main {
  width: 1760px;
  display: flex;

}

.NavBar_logo {
  width: 68px;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.NavBar_logo img {
  width: 68px;
  height: 48px;
}

.NavBar_List {
  width: 100%;
  display: flex;
  justify-content: flex-end;

}

.NavBar_List_Content {
  width: auto;
  height: 80px;
  font-size: 15px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  margin: 0px 10px;
  position: relative;
  transform: translateY(4px);

}

.active_List {
  width: 100%;
  height: 4px;
  position: absolute;
  bottom: 4px;
  left: 0;
  background-color: #597BE5;
}

.Secondary_Menu {
  width: 100%;
  height: 240px;
  display: flex;
  justify-content: center;
  background-color: rgba(7, 16, 39, 0.9);
}

.Secondary_Menu_Data {
  width: 1200px;
  padding: 40px 0;
}

.Secondary_Menu_title {
  display: flex;
}

.Secondary_Menu_Icon {
  width: 28px;
  height: 28px;
}

.Secondary_Menu_title_Text {
  height: 30px;
  font-size: 30px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 30px;
  margin-left: 20px;
}

.Secondary_Menu_List {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  font-size: 18px;
  font-family: Noto Sans JP;
  font-weight: 500;
  color: #FFFFFF;
  line-height: 18px;
  padding: 0 48px;
}

.Secondary_Menu_List_Data {
  margin-top: 40px;
  height: 18px;
  flex: 0 0 calc(33.33% - 10px);
}

@media only screen and (min-width: 1300px) and (max-width: 1760px) {
  .NavBar_Main {
    width: 1200px;
    display: flex;
  }

  .Secondary_Menu_Data {
    width: 900px;
  }
}

@media only screen and (min-width: 768px) and (max-width: 1299px) {
  .NavBar_Main {
    width: 700px;
    display: flex;
  }

  .Secondary_Menu_Data {
    width: 680px;
  }

  .Secondary_Menu_List_Data {
    text-align: center;
  }
}

@media only screen and (max-width: 767px) {
  .Nav_Bar_h {
    height: auto;
  }

  .Nav_Bar_List_data {
    display: flex;
    align-items: center;
    height: 100%;
  }

  .NavBar_Main {
    width: 80%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;

  }

  .Secondary_Menu {
    height: auto;
    background-color: rgba(7, 16, 39, 0.1);
  }

  .Secondary_Menu_Data {
    width: 80%;
    display: flex;
    flex-wrap: wrap;

  }

  .Secondary_Menu_List {
    width: 100%;
    padding: 0;
  }

  .Secondary_Menu_title_Text {
    width: 100%;
  }

  .Secondary_Menu_List_Data {
    text-align: left;
    margin-top: 30px;
    display: flex;
    flex-wrap: wrap;
    flex: 0 0 calc(100% - 10px);
  }

  .Secondary_Menu_title {
    width: 100%;
  }

  .nav_bar_button {
    width: 40px;
    height: 40px;
  }

  .menu_Btn {
    width: 40px;
    height: 40px;
    display: block;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    border: 1px solid white;
    border-radius: 5px;
  }

  .NavBar_Main_List {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .NavBar_List_Content {
    width: 100%;
    height: 50px;
  }

  .NavBar_List {
    flex-wrap: wrap;
  }
}</style>