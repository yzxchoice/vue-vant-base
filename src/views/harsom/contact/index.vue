<template>
  <div class="home">
    <img src="../../../assets/contact/联系我们头图@2x.png" alt="" />

    <div class="list">
      <div class="item header">
        <div class="title1">上海总部</div>
        <div class="title2">SHANGHAI HEADQUARTER</div>
        <p>地址：上海市浦东新区金桥现代产业服务园区4号楼2楼（总部）</p>
        <p>电话：021-50117066</p>
      </div>
      <div class="item">
        <div class="title2">陕西办事处</div>
        <p>地址：陕西省西安市唐延路11号禾盛京广E座1503室</p>
        <p>电话：17791900022</p>
      </div>
      <div class="item">
        <div class="title2">四川办事处</div>
        <p>地址：四川省成都市武侯区奥克斯广场9栋2204</p>
        <p>电话：18909229508</p>
      </div>
      <div class="item">
        <div class="title2">贵州办事处</div>
        <p>
          地址：贵州省贵阳市云岩区宝山北路133号西湖花园酒店停车场内创意工坊三楼
        </p>
        <p>电话：13639149192</p>
      </div>
      <div class="item">
        <div class="title2">安徽办事处</div>
        <p>地址：安徽省合肥市蜀山区岳西路与黄山路交口汇丰大厦808</p>
        <p>电话：13371909223</p>
      </div>
      <div class="item">
        <div class="title2">河南办事处</div>
        <p>地址：河南省郑州市中原区电厂路华强城市广场一期六单元605</p>
        <p>电话：13701910885</p>
      </div>
      <div class="item">
        <div class="title2">山东办事处</div>
        <p>地址：山东省济南市槐荫区发祥巷二区7号楼一单元2210室</p>
        <p>电话：13651717222</p>
      </div>
    </div>

    <img src="../../../assets/contact/办事处分布图@2x.png" alt="" />

    <div class="copyright">
      <img src="../../../assets/achievements/底部vi显示备份 3@2x.png" alt="" />
    </div>
  </div>
</template>

<script>
// 使用vant 组件

export default {
  name: 'Home',
  components: {},
  data() {
    return {}
  },
  created() {},

  methods: {}
}
</script>
<style lang="less" scoped>
.home {
  /** 审查元素，这个样式会转换为 font-size: 4.267vw; */
  //   font-size: 14px;
  background-color: #f9fafb;
  img {
    display: block;
    width: 100%;
  }
  .list {
    background-color: #fff;
    margin: 0 4px 4px 4px;
    border-bottom-left-radius: 10px; //左上角
    border-bottom-right-radius: 10px; //左下角
  }
  .item {
    padding: 0 26px 24px;
    border-bottom: 2px solid #efefef;
    &:nth-last-child(1) {
      border: 0;
    }
    .title1 {
      font-size: 24px;
      font-weight: 600;
      line-height: 33px;
      color: #000000;
    }
    .title2 {
      margin: 23px 0 10px;
      font-size: 16px;
      font-weight: 500;
      line-height: 22px;
      color: #0a0a0a;
      &.header {
        margin: 11px 20px;
      }
    }
    p {
      font-size: 14px;
      font-weight: 400;
      line-height: 22px;
      color: #303232;
    }
  }
  .copyright {
    margin: 51px 98px;
  }
}
</style>
