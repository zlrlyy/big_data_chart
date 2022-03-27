<template>
  <div>
    <h2>图表</h2>
    <div class="chart">
      
    </div>
  </div>
</template>

<script>
import {inject} from 'vue'

export default {
  setup(){
    const echarts = inject('echarts')
    const axios = inject('axios')
    console.log(echarts);
    console.log(axios);
  }

}
</script>

<style>

</style>