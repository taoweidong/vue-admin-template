<template>
  <section class="app-main">
    <!-- 其中transition 定义了页面之间切换动画，可以根据自己的需求，自行修改转场动画。相关文档 。
    默认提供了fade和fade-transform两个转场动画，具体 css 实现见transition.scss 。
    如果需要调整可在AppMain.vue 中调整transition 的 name。 -->
    <transition name="fade-transform" mode="out-in">
      <router-view :key="key" />
    </transition>
  </section>
</template>

<script>
export default {
  name: 'AppMain',
  computed: {
    /**
     *此方法解决不同操作使用同一组件时切换并不会触发 vue 的 created 或者 mounted 钩子的问题
     */
    key() {
      return this.$route.path
    }
  }
}
</script>

<style scoped>
.app-main {
  /*50 = navbar  */
  min-height: calc(100vh - 50px);
  width: 100%;
  position: relative;
  overflow: hidden;
}
.fixed-header + .app-main {
  padding-top: 50px;
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
