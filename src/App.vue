<template>
  <router-view/>
</template>

<script>
import {provide} from "vue"
import * as echarts from "echarts" 
import axios from 'axios'

export default {
  setup(){
    // provide('随便名字','内容')
    provide("echarts",echarts)
    provide("axios",axios)
  }  
}
</script>

<style lang="less">
*{
  margin: 0px;
  padding: 0px;
}
body{
  background: url(~@/assets/img/bg.png) top center no-repeat;
}
</style>
