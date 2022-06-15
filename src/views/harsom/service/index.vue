<template>
  <div class="home">
    <div class="headerimg">
      <!-- <img src="../../../assets/servicesupport/产品服务头图.png" alt="" /> -->
    </div>

    <div class="card">
      <div class="titleimg1">
        <img
          src="../../../assets/servicesupport/一站式 产品服务解决方案备份@2x.png"
          alt=""
        />
      </div>
      <p>
        迪乐姆秉承“以客户为中心”的理念，服务网点遍及全国29个城市，为广大客户全方位提供优质的
        <span> “一站式产品服务解决方案”。 </span>
      </p>
      <img src="../../../assets/servicesupport/一站式图@2x.png" alt="" />
    </div>

    <div class="title">
      <img src="../../../assets/servicesupport/01产品资源@2x.png" alt="" />
    </div>

    <div class="card">
      <p>
        迪乐姆人工智能课程，以信息科技课程标准为依据，符合育人为先，科学原理与实践应用并重，鼓励“做中学”、“用中学”、“创中学”的课程要求，是学校课程的有效补充。
      </p>
      <div class="titleimg first">
        <img src="../../../assets/servicesupport/课程体系标签@2x.png" alt="" />
      </div>
      <p>
        迪乐姆人工智能课程体系，以AI素养提升为核心目标，促进学生核心素养发展。
      </p>
      <img
        src="../../../assets/servicesupport/12345插图@2x.png"
        alt=""
        class="feature"
      />
      <div class="titleimg">
        <img src="../../../assets/servicesupport/课程资源标签@2x.png" alt="" />
      </div>
      <p>
        为了全方位保障教学有效落地，迪乐姆提供完备的课程资源，为非专业教师降低技术难度，为技术老师降低教学难度。
      </p>
      <img
        src="../../../assets/servicesupport/课程资源插图@2x.png"
        alt=""
        class="feature"
      />
      <div class="titleimg">
        <img src="../../../assets/servicesupport/教学硬件标签@2x.png" alt="" />
      </div>
      <p>教学硬件套装能够满足不同课程的不同需求，提升学生的创新思维及能力。</p>
      <img
        src="../../../assets/servicesupport/硬件产品-图@2x.png"
        alt=""
        class="feature"
      />
      <div class="titleimg">
        <img src="../../../assets/servicesupport/软件平台标签@2x.png" alt="" />
      </div>
      <img
        src="../../../assets/servicesupport/软件平台插图@2x.png"
        alt=""
        class="feature"
      />
    </div>
    <div class="title">
      <img src="../../../assets/servicesupport/空间建设标签@2x.png" alt="" />
    </div>
    <div class="preview">
      <div
        v-for="(item, index) in thumbimages"
        :key="index"
        @click="preview(index)"
      >
        <img :src="item" alt="" />
      </div>
    </div>

    <div class="title">
      <img src="../../../assets/servicesupport/服务支持-标签@2x.png" alt="" />
    </div>

    <div class="card">
      <p>
        迪乐姆人工智能课程，以信息科技课程标准为依据，符合育人为先，科学原理与实践应用并重，鼓励“做中学”、“用中学”、“创中学”的课程要求，是学校课程的有效补充。
      </p>
      <img
        src="../../../assets/servicesupport/服务@2x.png"
        alt=""
        class="support"
      />
      <!-- <img
        src="../../../assets/servicesupport/编组 7备份@2x.png"
        alt=""
        class="support"
      />
      <img
        src="../../../assets/servicesupport/编组 7备份 2@2x.png"
        alt=""
        class="support"
      />
      <img
        src="../../../assets/servicesupport/编组 7备份 3@2x.png"
        alt=""
        class="support"
      /> -->
    </div>

    <div class="copyright">
      <img src="../../../assets/achievements/底部vi显示备份 3@2x.png" alt="" />
    </div>
  </div>
</template>

<script>
// 使用vant 组件
import { ImagePreview } from 'vant'
export default {
  name: 'Home',
  components: {},
  data() {
    return {
      images: [
        require('../../../assets/servicesupport/1@2x.png'),
        require('../../../assets/servicesupport/841638425138_.pic@2x.png'),
        require('../../../assets/servicesupport/3@2x.png'),
        require('../../../assets/servicesupport/4@2x.png'),
        require('../../../assets/servicesupport/4@2x(1).png'),
        require('../../../assets/servicesupport/6@2x.png'),
        require('../../../assets/servicesupport/7@2x.png'),
        require('../../../assets/servicesupport/8@2x.png'),
        require('../../../assets/servicesupport/9@2x.png')
      ],
      thumbimages: [
        require('../../../assets/servicesupport/s1@2x.png'),
        require('../../../assets/servicesupport/s2@2x.png'),
        require('../../../assets/servicesupport/s3@2x.png'),
        require('../../../assets/servicesupport/s4@2x.png'),
        require('../../../assets/servicesupport/s5@2x.png'),
        require('../../../assets/servicesupport/s6@2x.png'),
        require('../../../assets/servicesupport/s7@2x.png'),
        require('../../../assets/servicesupport/s8@2x.png'),
        require('../../../assets/servicesupport/s9@2x.png')
      ]
    }
  },
  created() {},

  methods: {
    preview(index) {
      ImagePreview({
        images: this.images,
        startPosition: index
      })
    }
  }
}
</script>
<style lang="less" scoped>
.home {
  /** 审查元素，这个样式会转换为 font-size: 4.267vw; */
  //   font-size: 14px;
  background-color: #eaf1f7;
  //   padding-top: 219px;
  .headerimg {
    width: 100%;
    height: 252px;
    margin-bottom: -50px;
    background-image: url(../../../assets/servicesupport/产品服务头图@2x.png);
    background-repeat: no-repeat;
    background-size: cover;
  }
  img {
    display: block;
    width: 100%;
  }
  .small {
    margin-top: 8px;
    font-size: 10px;
    line-height: 14px;
    text-align: right;
  }
  .preview {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 16px;
    img {
      width: 100%;
      height: 100%;
    }
    div {
      width: 111px;
      height: 77px;
      margin-bottom: 6px;
      overflow: hidden;
      background-color: #cccccc;
      border-radius: 4px;
    }
  }
  .titlebox {
    padding: 13px 14px;
    margin: 12px 16px 0;
    color: #ffffff;
    background: linear-gradient(127deg, #3596ff 0%, #054beb 100%);
    border-radius: 8px;
    .line1 {
      font-size: 20px;
      font-weight: 600;
      line-height: 28px;
    }
    .line2 {
      margin-top: 8px;
      font-size: 14px;
      font-weight: 400;
      line-height: 24px;
    }
  }
  .title {
    margin: 24px 16px 0 7px;
  }
  .card {
    padding: 14px;
    margin: 18px 16px 0;
    background: #ffffff;
    border-radius: 10px;
    box-shadow: 4px 4px 6px 0 rgba(115, 140, 187, 0.32);
    .titleimg1 {
      margin-top: 4px;
      margin-bottom: 14px;
      img {
        width: 236px;
      }
    }
    .titleimg {
      width: 80px;
      height: 28px;
      margin: 30px 0 7px;
      &.first {
        margin: 0 0 17px;
      }
    }
    p {
      &:nth-child(1) {
        margin: 0 0 15px;
      }

      margin: 15px 0;
      span {
        color: #3263ff;
      }
    }
    .secend {
      i {
        display: inline-block;
        width: 10px;
        height: 10px;
        background: #5c5c5c;
        border-radius: 50%;
      }
      span {
        margin-left: 10px;
      }
    }
  }
  //   .feature {
  //     margin-top: 10px;
  //     margin-bottom: 30px;
  //   }
  .support {
    margin-bottom: 7px;
  }
  .copyright {
    margin: 51px 98px;
  }
}
</style>
