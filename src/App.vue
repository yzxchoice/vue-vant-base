<!--
 * @Description: 文件说明
 * @FilePath: \vue-base\src\App.vue
-->
<template>
  <div id="app">
    <transition :name="transitionName">
      <navigation>
        <router-view class="router" />
      </navigation>
    </transition>
  </div>
</template>
<script>
export default {
  data() {
    return {
      transitionName: 'van-slide-right'
    }
  },
  created() {
    this.$navigation.on('forward', () => {
      this.transitionName = 'van-slide-right'
    })
    this.$navigation.on('back', () => {
      this.transitionName = 'van-slide-left'
    })
  }
}
</script>

<style lang="less">
.font('Alibaba-PuHuiTi-Medium');
#app {
  height: 100vh;
  font-family: PingFangSC-Regular, sans-serif;
  background-color: #eaf1f7;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: @gray;
  font-size: 14px;
  font-family: PingFangSC-Regular, PingFang SC;
  // font-weight: 400;
  line-height: 2;
  text-align: justify;
  word-wrap: break-word;
  .van-swipe__indicator {
    width: 10px;
    height: 4px;
    border-radius: 0;
    background-color: #d8d8d8;
  }
  .van-swipe__indicator--active {
    background-color: #26b1f2;
    opacity: 1;
  }
  .video-js {
    width: 100%;
    height: auto;
    padding-bottom: 75%;
    margin: 16px 0;
    overflow: hidden;
    border-radius: 10px;
  }
  .vjs-big-play-button {
    width: 1.63332em;
    height: 1.63332em;
    border-radius: 50%;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    border: 0;
  }
}

p {
  margin: 0;
}

/** 解决路由切换动画上下闪动问题 */
.router {
  position: absolute;
  top: constant(safe-area-inset-top);
  top: env(safe-area-inset-top);
  width: 100%;
  transition: all 0.377s ease;
  backface-visibility: hidden;
}
.van-tabs {
  margin: 8px;
}
.van-tabs .van-tabs__nav {
  background-color: transparent;
}
.van-tab.van-tab--active {
  background-color: #2b71fa;
  color: #ffffff;
  border-radius: 4px;
  .van-tab__text {
    color: #ffffff;
  }
}
.van-tabs__nav--line.van-tabs__nav--complete {
  padding-right: 0;
  padding-left: 0;
}
.van-tab .van-tab__text {
  // margin: 15px 16px;
  font-size: 12px;
  color: #6e6f71;
  font-weight: 500;
}
.van-tabs .van-tabs__line {
  background-color: transparent;
}
.van-tabs__content {
  padding: 8px;
}
.van-tabs--line .van-tabs__wrap {
  height: 28px !important;
}
</style>
