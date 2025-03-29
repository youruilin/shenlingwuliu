<template>
  <section class="app-main">
    <transition
      name="fade-transform"
      mode="out-in"
    >
      <router-view :key="key" />
    </transition>
    <div style="font-size:14px;color:#BAC0CD;text-align:center;padding-bottom:20px;background-color:#F3F4F7;position:absolute;bottom:0;left:0%;width:100%;padding-top:20px">
      游瑞林個人作品demo
      <span style="margin-left:20px">版权所有Copyright 2006-2025  All Rights Reserved</span>
      <span style="margin-left:20px">プロジェクトのデモは、ご覧・ご参考のみです。</span>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AppMain',
  computed: {
    key() {
      return this.$route.path
    }
  }
}
</script>
<style scoped>
.app-main {
  /*50 = navbar  */
  min-height: calc(100vh - 0px);
  width: 100%;
  position: relative;
  /* overflow: hidden; */
  overflow-x: hidden;
  /* 解决iframe嵌套出现光滚动条问题 */
  /* overflow-y: scroll; */
  /* background-color: #fff; */
  background-color: #f3f4f7;
}
.fixed-header + .app-main {
  padding-top: 46px;
}
</style>

<style lang="scss">
// fix css style bug in open el-dialog
.el-popup-parent--hidden {
  .fixed-header {
    padding-right: 15px;
  }
}
</style>
