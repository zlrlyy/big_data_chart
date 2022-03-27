<template>
  <div class="item">
    <!-- 设置插槽 -->
    <slot></slot>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>
  .item{
    height: 5.9rem;
    margin: 0.2rem;
    border: 1px solid rgb(22, 22, 90);
    background-color: rgba(10, 40, 71, 0.7);
  }
</style>