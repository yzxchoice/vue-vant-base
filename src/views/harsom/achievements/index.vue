<template>
  <div class="home">
    <img src="../../../assets/achievements/学术成果头图.png" alt="" />
    <div class="titlebox">
      <div class="line1">智能时代，我们携手共进</div>
      <div class="line2">
        人工智能时代，学生需要从死记硬背的灌输式教育中解放出来。培养学生的智能社会责任感、思辨能力、实践能力、创新能力等一系列机器无法具备的核心能力与素养，是人工智能教育的重要使命。迪乐姆自主建构了从人工智能课程核心素养、课程研发到教师培养、教学落地等适用于人工智能各环节的理论模型，并经过实践的反复印证，形成了完整的教学理论闭环。
      </div>
    </div>
    <div class="title">
      <img src="../../../assets/achievements/学术标题1.png" alt="" />
    </div>

    <div class="card">
      <div class="xueshu1">
        <img src="../../../assets/achievements/人工智能教育理念.png" alt="" />
      </div>

      迪乐姆人工智能教育，以编程、人工智能知识为载体，融合思维能力培养目标，运用思维型教学方法，引导学生通过项目式学习和动手实践相结合的方式，培养学生跨学科解决问题能力，支持学生核心素养的全面发展。
      <img
        src="../../../assets/achievements/人工智能教育理念配图.png"
        alt=""
        class="feature"
      />
      迪乐姆创新性地提出，人工智能核心素养由智能意识、智能观念、智能思维与智能实践力构成。学生在从事人工智能活动时，良好的智能意识能为其提供运用人工智能的相关思想、方法、技术、应用解决问题的内在动机；良好的智能观念则为学生正确使用人工智能提供了保障、明确了方向；良好的智能思维为学生提供了解决问题的方法路径；良好的智能实践力则为学生提供了问题解决所需要的实现路径；而问题解决所形成的经验、成就感等，又进一步促进了智能意识的发展。
      <div class="small">
        <p>——《中小学人工智能课程核心素养构建》</p>
        <p>发表于《中小学信息技术教育》杂志</p>
      </div>

      <p></p>
    </div>
    <div class="title">
      <img src="../../../assets/achievements/学术标题2.png" alt="" />
    </div>
    <div class="card">
      <div class="xueshu2">
        <img src="../../../assets/achievements/副标题备份 5.png" alt="" />
      </div>
      迪乐姆人工智能课程，以学生的问题解决能力为导向，重点关注学生的分解问题和抽象聚焦的计算思维能力，从底层思维方法出发，全面提高学生的基础认知能力，在实际课堂教学的AI应用场景中，通过思维型教学提高学生的创新意识与能力。
      <img
        src="../../../assets/achievements/编组 3.png"
        alt=""
        class="feature"
      />
      <div class="xueshu3">
        <img src="../../../assets/achievements/副标题备份 4.png" alt="" />
      </div>
      迪乐姆根据国内外先进课程教学理论，创新提出支持直接落地的FCT教学法，即以思维为中心，以5C为基本环节，以5F为基本策略，将“上好人工智能课”细化为可操作的教学步骤与可习得的教学模式，做好教学理论最后一公里。
      <img
        src="../../../assets/achievements/编组 4.png"
        alt=""
        class="feature"
      />
      <div class="xueshu4">
        <img src="../../../assets/achievements/副标题备份 3.png" alt="" />
      </div>
      迪乐姆聚焦“专业师培”这一难题，从顶层设计入手，搭建了KOT人工智能教师胜任力模型，并绘制了教师成长的发展路线，明确了人工智能教师个发展阶段的能力标准。
      <img
        src="../../../assets/achievements/编组 5.png"
        alt=""
        class="feature"
      />
      <div class="xueshu1">
        <img src="../../../assets/achievements/副标题备份.png" alt="" />
      </div>

      <img
        src="../../../assets/achievements/编组 18.png"
        alt=""
        class="feature"
      />
    </div>

    <div class="copyright">
      <img src="../../../assets/coursesystem/copyright.png" alt="" />
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
  background-color: #eaf1f7;
  img {
    width: 100%;
    display: block;
  }
  .small {
    margin-top: 10px;
    font-size: 10px;
    line-height: 22px;
    text-align: right;
    margin-bottom: 10px;
  }

  .xueshu1 {
    margin-top: 4px;
    margin-bottom: 14px;
    width: 138px;
  }
  .xueshu2 {
    margin-top: 4px;
    margin-bottom: 14px;
    width: 136px;
  }
  .xueshu3 {
    margin-top: 4px;
    margin-bottom: 14px;
    width: 96px;
  }
  .xueshu4 {
    margin-top: 4px;
    margin-bottom: 14px;
    width: 84px;
  }
  .titlebox {
    margin: 12px 16px 0;
    padding: 13px 14px;
    background: linear-gradient(127deg, #3596ff 0%, #054beb 100%);
    border-radius: 8px;
    color: #ffffff;
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
    margin: 18px 16px 0;
    background: #ffffff;
    box-shadow: 4px 4px 6px 0px rgba(115, 140, 187, 0.32);
    border-radius: 10px;
    padding: 14px 14px 8px 14px;
    .secend {
      i {
        display: inline-block;
        width: 10px;
        height: 10px;
        border-radius: 50%;
        background: #5c5c5c;
      }
      span {
        margin-left: 10px;
      }
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
