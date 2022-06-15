<template>
  <div class="home">
    <img src="../../../assets/teacherservice/师训服务头图@2x.png" alt="" />
    <div class="titlebox">
      <div class="line2">
        普及人工智能教育，教师是关键。目前，AI教师大部分非专业出身，缺乏必要的专业知识体系、实操技能。同时，人工智能作为一门新的交叉学科，缺乏现成的教学范例。提升教师AI素养、教学效果、学业质量，需要做好课程落地的最后一公里。
      </div>
    </div>
    <div class="title">
      <img src="../../../assets/teacherservice/教师标题1@2x.png" alt="" />
    </div>

    <div class="card">
      迪乐姆聚焦“专业师培”这⼀难题，从顶层设计⼊⼿，搭建了⼈⼯智能教师专业标准，并建构出总体培养目标及具体学习内容。
      <img
        src="../../../assets/teacherservice/位图@2x.png"
        alt=""
        class="feature"
        @click="preview(0)"
      />
    </div>

    <div class="title">
      <img src="../../../assets/teacherservice/教师标题2@2x.png" alt="" />
    </div>

    <div class="card">
      基于教师培养的实际需求，有如下三种合作模式：
      <img
        src="../../../assets/teacherservice/紫@2x.png"
        alt=""
        class="feature"
        @click="preview(1)"
      />
      <img
        src="../../../assets/teacherservice/黄@2x.png"
        alt=""
        class="feature"
        @click="preview(2)"
      />
      <img
        src="../../../assets/teacherservice/红@2x.png"
        alt=""
        class="feature"
        @click="preview(3)"
      />

      三种培养模式在目标和内容上，呈包含式递进关系，即中期系统培训包含短期专题培训所有的目标和内容，长期定制培训包含中期培训所有的目标和内容，每期的培养在标准方案的基础上，可以做<span>个性化定制，以保证效果的最优化</span>。
    </div>

    <div class="title">
      <img src="../../../assets/teacherservice/教师标题3@2x.png" alt="" />
    </div>

    <div class="card">
      三阶段两场景立体师训，全方位支持教师成长和教学落地。
      <img
        src="../../../assets/teacherservice/3阶段图@2x.png"
        alt=""
        class="feature"
      />
      <img
        src="../../../assets/teacherservice/编组 13备份@2x.png"
        alt=""
        class="feature"
      />
      <img
        src="../../../assets/teacherservice/编组 13@2x.png"
        alt=""
        class="feature"
      />
    </div>

    <div class="linkbox">
      <div class="left">
        <img src="../../../assets/teacherservice/链接1@2x.png" alt="" />
      </div>
      <div class="right">
        <img src="../../../assets/teacherservice/链接1@2x.png" alt="" />
      </div>
    </div>

    <div class="card">
      <div class="xueshu2">
        <img src="../../../assets/teacherservice/副标题备份 6@2x.png" alt="" />
      </div>
      集中培训内容分为公共课、专业课、教研课三大模块。公共课为新手教师提供了人工智能的通用知识、教学理论、观念等；专业课能帮助新手教师尽快掌握授课所需的AI实操技能；教研课则能针对实际课程的掌握，切实提高教师教学展示效果。
      <img
        src="../../../assets/teacherservice/3种课程表@2x.png"
        alt=""
        class="feature"
        @click="preview(4)"
      />
      <div class="xueshu3">
        <img src="../../../assets/teacherservice/副标题备份 7@2x.png" alt="" />
      </div>
      教学指导能更好的助力AI教师持续成长，提升人工智能课程胜任力，并及时跟进学校在课程落地实施过程中遇到的问题，提供指导方案。
      <img
        src="../../../assets/teacherservice/卡片内容@2x.png"
        alt=""
        class="feature"
      />
      <div class="xueshu4">
        <img src="../../../assets/teacherservice/副标题备份 9@2x.png" alt="" />
      </div>
      <span>教学能力考核：</span
      >以教学技能比赛等方式对教师人工智能教学能力进行考核评价
      <img
        src="../../../assets/teacherservice/编组 4@2x.png"
        alt=""
        class="feature"
      />
      <span>学生创新竞赛：</span
      >制定区域学生创新比赛规则，组织进行比赛活动、学生作品评审
      <img
        src="../../../assets/teacherservice/编组 5@2x.png"
        alt=""
        class="feature"
      />
      <span>教师人工智能论文与教学设计比赛：</span
      >各区域教师投稿，专家评委审稿，联合当地教育局监章，激活教师参赛动力，促进教研能力提升。
    </div>

    <div class="title">
      <img src="../../../assets/teacherservice/学术标题1备份@2x.png" alt="" />
    </div>

    <div>
      <van-swipe class="teacher-swipe" :loop="false" :width="345" :height="350">
        <van-swipe-item>
          <img src="../../../assets/teacherservice/案例1@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/teacherservice/案例2@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/teacherservice/案例3@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/teacherservice/案例4@2x.png" alt="" />
        </van-swipe-item>
      </van-swipe>
    </div>

    <div class="copyright">
      <img src="../../../assets/achievements/底部vi显示备份 3@2x.png" alt="" />
    </div>
  </div>
</template>

<script>
// 使用vant 组件
import { Tab, Tabs, Swipe, SwipeItem, ImagePreview } from 'vant'

export default {
  name: 'Home',
  components: {
    [Tab.name]: Tab,
    [Tabs.name]: Tabs,
    [Swipe.name]: Swipe,
    [SwipeItem.name]: SwipeItem
  },
  data() {
    return {
      images: [
        require('../../../assets/teacherservice/位图@2x.png'),
        require('../../../assets/teacherservice/紫@2x.png'),
        require('../../../assets/teacherservice/黄@2x.png'),
        require('../../../assets/teacherservice/红@2x.png'),
        require('../../../assets/teacherservice/3种课程表@2x.png'),
        require('../../../assets/teacherservice/案例2@2x.png'),
        require('../../../assets/teacherservice/案例3@2x.png'),
        require('../../../assets/teacherservice/案例4@2x.png')
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
  .teacher-swipe {
    margin: 10px 0 10px 16px;
  }
  .linkbox {
    position: relative;
    .left {
      position: absolute;
      width: 12px;
      height: 42px;
      left: 30px;
      bottom: -30px;
    }
    .right {
      position: absolute;
      width: 12px;
      height: 42px;
      right: 30px;
      bottom: -30px;
    }
  }
  .teacher-swipe .van-swipe-item {
    font-size: 20px;
    line-height: 150px;
    color: #ffffff;
    text-align: center;
    img {
      width: 96%;
    }
  }
  img {
    display: block;
    width: 100%;
  }
  .small {
    margin-top: 10px;
    margin-bottom: 10px;
    font-size: 10px;
    line-height: 22px;
    text-align: right;
  }

  .xueshu1 {
    width: 138px;
    margin-top: 4px;
    margin-bottom: 14px;
  }
  .xueshu2 {
    width: 208px;
    margin-top: 4px;
    margin-bottom: 14px;
  }
  .xueshu3 {
    width: 208px;
    margin-top: 4px;
    margin-bottom: 14px;
  }
  .xueshu4 {
    width: 208px;
    margin-top: 4px;
    margin-bottom: 14px;
  }
  .titlebox {
    padding: 13px 14px;
    margin: 12px 16px 0;
    color: #ffffff;
    background: linear-gradient(126deg, #8c9eff 0%, #1935ca 100%);
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
    padding: 14px 14px 8px;
    margin: 18px 16px 0;
    background: #ffffff;
    border-radius: 10px;
    box-shadow: 4px 4px 6px 0 rgba(115, 140, 187, 0.32);
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
    span {
      color: #455dde;
    }
  }
  .feature {
    margin-top: 18px;
    margin-bottom: 29px;
  }
  .copyright {
    margin: 51px 98px;
  }
}
</style>
