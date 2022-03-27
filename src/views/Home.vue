<template>
  <div id="content">
    <header>
      <h1>
        郑礼儒吊炸天数据可视化
      </h1>
    </header>
    <!-- 主题内容 -->
    <main id="container">
      <!-- 左容器 -->
      <section class="left-container">
        <item-page>
          <item-one/>
        </item-page>
        <item-page>
          <item-two/>
        </item-page>
      </section>
      <section class="center-container"></section>
      <section class="right-container">
        <item-page>
          <item-three/>
        </item-page>
        <item-page>
          <item-four/>
        </item-page>
      </section>
    </main>
  </div>
</template>

<script>
import ItemPage from '@/components/ItemPage.vue'
import ItemOne from '../components/ItemOne.vue'
import ItemTwo from '../components/ItemTwo.vue'
import ItemThree from '../components/ItemThree.vue'
import ItemFour from '../components/ItemFour.vue'

export default {
  name: 'Home',
    components:{
      ItemPage,
      ItemOne,
      ItemTwo,
      ItemThree,
      ItemFour,
    }
}
  
</script>

<style lang="less" scoped>
#content{
  overflow: hidden;
  header{
  width: 100%;
  height: 1rem;
    h1{
      font-size: .5rem;
      color: #fff;
      text-align: center;
      line-height: 1rem;
    }
  }
  #container{
    min-width: 1200px;
    max-width: 2048px;
    margin: 0 auto;
    padding: 0.12rem 0.12rem 0;
    border: 1px solid red;
    display: flex;
    .left-container,.right-container{
      flex: 3;
    }
    .center-container{
      flex:5;
      height: 12rem;
      margin: 0.2rem;
      border: 1px solid rgb(22, 22, 90);
      background-color: rgba(10, 40, 71, 0.7);
    }
  }
}
</style>
