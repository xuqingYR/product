<template>
  <div id="app">
    <top />
    <name />
    <router-view/>
  </div>
</template>

<script>
import top from './components/top.vue'
import name from './components/name.vue'
export default {
  name: 'App',
  data(){
    return{

    }
  },
  components:{
    top,
    name
  }
}
</script>

<style>
html, body, div, span, applet, object, iframe,h1, h2, 
h3, h4, h5, h6, p, blockquote, pre,abbr, address, cite, code,del, dfn, 
em, img, ins,kbd, q, s, samp,small, strong, sub, sup, var,b,u, i,center,dl, dt, dd, 
ol, ul, li,fieldset, form, label, legend,table, caption, tbody, 
tfoot,thead,tr, th, td,article, aside, canvas, details,embed, figcaption, 
figure, footer, header, hgroup, menu, nav, section, summary,time, mark, 
audio, video {
    margin:0;
    padding:0;
    border:0;
    outline:0;
    font-size:100%;
    font: inherit;
}
article, aside, details, figcaption, figure,
footer, header, hgroup, menu, nav, section {
display: block;
}
body {
      font-size: 14px;
    background-color: #F2F2F2 ;
    font-family: "Helvetica Neue",Arial, Helvetica, "Hiragino Sans GB","Hiragino Sans GB W3",
    "Microsoft YaHei UI","Microsoft YaHei","WenQuanYi Micro Hei",sans-serif;
}
ol, ul{
  list-style: none;
}
blockquote, q{
  quotes: none;
}
blockquote:before, blockquote :after,
q:before, q:after{
  content: '';
  content: none;
}
a{
    color: inherit;
    text-decoration: none;
     
}

table {
    border-collapse:collapse;
    border-spacing:0;
}
 
input, select {
    vertical-align:middle;
}

/*css为clearfix，清除浮动*/
.clearfix::before,
.clearfix::after{
    content: "";
    height: 0;
    line-height: 0;
    display: block;
    visibility: hidden;
    clear: both;
}
.clearfix:after{clear:both;} 
.clearfix{ 
    *zoom:1;/*IE/7/6*/
}

</style>
