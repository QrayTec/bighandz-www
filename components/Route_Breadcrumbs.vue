<template >
  <div class="Route_Breadcrumbs">
    <div class="Route_Breadcrumbs_main">
      <div class="Parent_title">{{ Parent_title }}</div>

      <div class="Route_Breadcrumbs_to">
        <img src="~/assets/Route_Breadcrumbs/icon_right.png" alt="">
      </div>
      <div class="Route_Breadcrumbs_Index_title">{{Index_title}}</div>
    </div>
  </div>
</template>
<script>
import json from '~/Route_Breadcrumbs/Route_Breadcrumbs.json';
export default {
  data() {
    return {
      Parent_title:"",
      Index_title:""
    }
  },
  mounted(){
    this.getPageTitle()
  },
    methods: {
    getPageTitle() {
      const routePath = this.$route.path
      const page = json[routePath]
      if (typeof page === 'string') {
        return page
      } else if (page && page.name) {
        this.Parent_title=page.Parent_title
        this.Index_title=page.name
        return page.name
      } else {
        return 'Unknown Page'
      }
    }
  }
}

</script>
<style >
  .Route_Breadcrumbs_main{
    display: flex;
    align-items: center;
  }
  .Parent_title{
    height: 16px;
    font-size: 16px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 16px;
    opacity: 0.4;
  }
  .Route_Breadcrumbs_to{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0px 20px;
  }
  .Route_Breadcrumbs_Index_title{
    height: 16px;
    font-size: 16px;
    font-family: Noto Sans JP;
    font-weight: 400;
    color: #FFFFFF;
    line-height: 16px
  }
</style>