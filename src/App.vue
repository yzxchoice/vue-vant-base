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
.van-image-preview__image {
  background-color: #fff;
}
#app {
  height: 100vh;
  font-family: PingFangSC-Regular, sans-serif;
  font-family: PingFangSC-Regular, PingFang SC;
  font-size: 14px;
  // font-weight: 400;
  line-height: 2;
  color: @gray;
  text-align: justify;
  word-wrap: break-word;
  background-color: #eaf1f7;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  .van-image-preview__image {
    background-color: #fff;
  }
  .van-swipe__indicator {
    width: 10px;
    height: 4px;
    background-color: #d8d8d8;
    border-radius: 8px;
  }
  .van-swipe__indicator--active {
    background-color: #26b1f2;
    opacity: 1;
    border-radius: 8px;
  }
  .teacher-swipe .van-swipe__indicator {
    width: 4px;
  }
  .teacher-swipe .van-swipe__indicator--active {
    width: 20px;
  }
  .teacher-swipe .van-swipe__indicator--active {
    background-color: #4860e0;
    opacity: 1;
  }
  .video-js {
    width: 100%;
    height: auto;
    padding-bottom: 56%;
    margin: 16px 0;
    overflow: hidden;
    border-radius: 10px;
  }
  .vjs-big-play-button {
    top: 50%;
    left: 50%;
    width: 1.63332em;
    height: 1.63332em;
    border: 0;
    border-radius: 50%;
    transform: translate(-50%, -50%);
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
  color: #ffffff;
  background-color: #2b71fa;
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
  font-weight: 500;
  color: #6e6f71;
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
