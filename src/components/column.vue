<template>
  <div>
    <div class="column-wrap" v-for="item in menuList">
      <div class="img-wrap" :style=item.bg>
        <img :src=item.img>
      </div>
      <div class="content-wrap">
        <div class="title">
          {{item.title}}
        </div>
        <router-link class="options" v-for="spa in item.menu" :to="{ path: spa.url }">
          <span>{{spa.menuName}}</span>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  export default{
    props: {
      menuList: {
        type: Array,
        default: [{
          title: '404',
          img: '',
          menu: [{
            menuName: '404',
            url: '..'
          }]
        }]
      }
    },
    data () {
      return {}
    },
    mounted () {
      console.log(this.menuList)
    }
  }
</script>

<style scoped>
  .column-wrap {
    float: left;
    width: 290px;
    height: 120px;
    background: #fff;
    margin: 20px 10px 0 10px;
  }
  .img-wrap {
    float: left;
    width: 120px;
    height: 120px;
  }
  .content-wrap {
    float: left;
    width: 170px;
    height: 120px;
    background: #fff;
  }
  .content-wrap .title {
    font-style: normal;
    font-size: 20px;
    margin-left: 20px;
    height: 60px;
    line-height: 60px;
  }
  .content-wrap .options {
    float: left;
    margin-left: 20px;
    height: 30px;
  }
  .content-wrap .options span {
    display: block;
    font-size: 14px;
    font-family: "Blackoak Std";
    width: 65px;
    height: 30px;
    color: #3366CC;
  }

</style>
