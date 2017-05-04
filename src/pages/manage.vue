<template>
  <div>
    <div class="page-head">
      <div class="page-head-inner">
        <router-link :to="{path: '/'}">
          <img src="../assets/logo3.png" alt="logo">
        </router-link>
        <div class="head-menu">
          <span>资讯管理</span>
          <span>产品管理</span>
        </div>
      </div>
    </div>
    <div class="manage-wrap">
      123
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default{
    data () {
      return {}
    }
  }
</script>

<style scoped>
  .page-head {
    background: #339966;
    color: #fff;
    height: 50px;
    line-height: 50px;
    width: 100%;
  }
  .page-head-inner {
    width: 1100px;
    margin: 0 auto;
  }
  .page-head-inner .head-menu h2{
    margin: 0 30px;
    font-size: 22px;
  }
  .page-head-inner img{
    float: left;
    height: 50px;
  }
  .head-menu {
    float: left;
  }
  .head-menu span{
    float: left;
    height: 50px;
    line-height: 50px;
    margin: 0px 40px;
    font-size: 16px;
  }
</style>
