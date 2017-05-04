<template>
  <div>
    <div class="app-head">
      <div class="app-head-inner">
        <router-link :to="{path: '/'}">
          <img src="../assets/logo3.png" alt="logo">
        </router-link>
        <div class="head-menu">
          <h2>中远地产</h2>
        </div>
      </div>
    </div>

    <div class="index-wrap">
      <h2>请选择功能</h2>
      <hr>
      <div class="menu-wrap">
        <column :menuList="menuList"></column>
      </div>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  import Column from '../components/column.vue'
  export default{
    components: {
      Column
    },
    data () {
      return {
        menuList: [
          {
            title: '资讯',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715620711.png',
            bg: 'background: #2097c8',
            menu: [
              {
                menuName: '资讯管理',
                url: '/manage'
              }
            ]
          },
          {
            title: '产品',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715691085.png',
            bg: 'background: #ee6f51',
            menu: [
              {
                menuName: '店铺',
                url: '.'
              },
              {
                menuName: '店铺聚合',
                url: '..'
              },
              {
                menuName: '产品聚合',
                url: '..'
              }
            ]
          },
          {
            title: '订单',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715620710.png',
            bg: 'background: #fec653',
            menu: [
              {
                menuName: '订单管理',
                url: '..'
              }
            ]
          },
          {
            title: '会员',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715691084.png',
            bg: 'background: #89cd4c',
            menu: [
              {
                menuName: '会员管理',
                url: '..'
              }
            ]
          },
          {
            title: '贴吧',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715620709.png',
            bg: 'background: #35bea8',
            menu: [
              {
                menuName: '贴吧管理',
                url: '..'
              }
            ]
          },
          {
            title: '表单',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715620708.png',
            bg: 'background: #7281bf',
            menu: [
              {
                menuName: '表单管理',
                url: '..'
              },
              {
                menuName: '高级表单',
                url: '..'
              }
            ]
          },
          {
            title: '统计',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715620707.png',
            bg: 'background: #ee6f51',
            menu: [
              {
                menuName: '应用统计',
                url: '..'
              },
              {
                menuName: '短信统计',
                url: '..'
              }
            ]
          },
          {
            title: '子账号',
            img: 'http://7xkul3.com1.z0.glb.clouddn.com/1493715620705.png',
            bg: 'background: #fec653',
            menu: [
              {
                menuName: '子账号管理',
                url: '..'
              }
            ]
          }
        ]
      }
    }
  }
</script>

<style scoped>
  .app-head {
    background: #339966;
    color: #fff;
    height: 50px;
    line-height: 50px;
    width: 100%;
  }
  .app-head-inner {
    width: 1100px;
    margin: 0 auto;
  }
  .app-head-inner .head-menu h2{
    font-size: 22px;
  }
  .app-head-inner img{
    float: left;
    height: 50px;
  }
  .head-menu {
    float: left;
  }
  .head-menu h3{
    float: left;
    height: 50px;
    line-height: 50px;
    margin: 0px 40px;
    font-size: 16px;
  }
  .index-wrap {
    width: 1100px;
    margin: 0 auto;
    overflow: hidden;
  }
  .index-wrap h2 {
    width: 940px;
    height: 30px;
    margin: 0 auto;
    margin-top: 20px;
    padding-left: 22px;
    font-size: 20px;
    color: #999;
    font-weight: 550;
  }
  .index-wrap hr {
    width: 940px;
  }

  .menu-wrap {
    width: 940px;
    height: 700px;
    margin: 0 auto;
  }
</style>
