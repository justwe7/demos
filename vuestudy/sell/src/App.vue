<template>
  <div id="app" class="app">
    <!--<div class="header">
      头部
    </div>-->
    <tmpheader></tmpheader>
    <nav class="tab">
      <div class="tab-item">
        <a v-link="{path: '/goods'}">商品</a>
      </div>
      <div class="tab-item">
        <a v-link="{path: '/ratings'}">评价</a>
      </div>
      <div class="tab-item">
        <a v-link="{path: '/seller'}">商家</a>
      </div>
    </nav>
    <router-view class="content">
      内容
    </router-view>
  </div>
</template>

<script type="text/ecmascript-6">
  import header from './components/header/header.vue';
  export default {
    components: {
      'tmpheader': header
    }
  };
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .app
    .tab
      display: flex
      width: 100%
      height: 40px
      line-height: 40px
      .tab-item
        flex: 1
        text-align: center
</style>
