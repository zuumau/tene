<template>
  <div>
    <!--<div class="app-head">-->
      <!--<div class="app-head-inner">-->
        <!--<router-link :to="{path: '/'}">-->
          <!--<img src="../assets/logo2.png" alt="logo">-->
        <!--</router-link>-->
        <!--<div class="head-menu">-->
          <!--<h2>中远地产</h2>-->
        <!--</div>-->
      <!--</div>-->
    <!--</div>-->

    <div class="app-content">
      <keep-alive>
        <router-view></router-view>
      </keep-alive>
    </div>

    <div class="app-foot">
      <p>©2016-2018 嘉峪关中远房地产开发有限公司  ygjsw.org  陇ICP备15000507号-2</p>
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

<style>
  /* http://meyerweb.com/eric/tools/css/reset/
   v2.0 | 20110126
   License: none (public domain)
*/

  html, body, div, span, applet, object, iframe,
  h1, h2, h3, h4, h5, h6, p, blockquote, pre,
  a, abbr, acronym, address, big, cite, code,
  del, dfn, em, img, ins, kbd, q, s, samp,
  small, strike, strong, sub, sup, tt, var,
  b, u, i, center,
  dl, dt, dd, ol, ul, li,
  fieldset, form, label, legend,
  table, caption, tbody, tfoot, thead, tr, th, td,
  article, aside, canvas, details, embed,
  figure, figcaption, footer, header, hgroup,
  menu, nav, output, ruby, section, summary,
  time, mark, audio, video {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
  }
  /* HTML5 display-role reset for older browsers */
  article, aside, details, figcaption, figure,
  footer, header, hgroup, menu, nav, section {
    display: block;
  }
  body {
    line-height: 1;
  }
  ol, ul {
    list-style: none;
  }
  blockquote, q {
    quotes: none;
  }
  blockquote:before, blockquote:after,
  q:before, q:after {
    content: '';
    content: none;
  }
  table {
    border-collapse: collapse;
    border-spacing: 0;
  }
  a {
    color: inherit;
    text-decoration: none;
  }
  body {
    background: #f0f2f5;
    font-family: "Helvetica Neue",Helvetica,Arial,"Hiragino Sans GB","Hiragino Sans GB W3","Microsoft YaHei UI","Microsoft YaHei","WenQuanYi Micro Hei",sans-serif;
    font-size: 14px;
    color: #444;
  }

  .app-foot {
    text-align: center;
    height: 50px;
    line-height: 50px;
    width: 100%;
    background: #e3e4e8;
    clear: both;
    margin-top: 30px;
  }


</style>
