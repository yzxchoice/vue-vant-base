<template>
  <div class="home">
    <img src="../../../assets/coursesystem/课程体系-头图@2x.png" alt="" />
    <div class="title">
      <img src="../../../assets/coursesystem/课程-标题1@2x.png" alt="" />
    </div>

    <div class="card">
      <p>
        迪乐姆人工智能课程以点、线、面多维途径展开，满足基础普适、兴趣拓展、竞赛提升不同场景的教学需求，为处于不同年龄、不同基础、不同目标的学生人群打造系统的课程体系，完美融合现有教育生态。
      </p>
      <img
        src="../../../assets/coursesystem/特色学校概念图@2x.png"
        alt=""
        class="feature"
        @click="preview(0)"
      />
    </div>
    <div class="title">
      <img src="../../../assets/coursesystem/课程-标题2@2x.png" alt="" />
    </div>
    <div class="card">
      <p>
        迪乐姆人工智能课程，以信息科技课程标准为依据，符合育人为先，科学原理与实践应用并重，鼓励“做中学”、“用中学”、“创中学”的课程要求，是学校课程的有效补充。
      </p>
      <img
        src="../../../assets/coursesystem/带小迪的课程表@2x.png"
        alt=""
        class="feature"
        @click="preview(1)"
      />
    </div>
    <div class="title">
      <img src="../../../assets/coursesystem/课程-标题3@2x.png" alt="" />
    </div>
    <div class="card">
      <p>
        迪乐姆人工智能课程，以TPI课程建构理论为依据，融合科学、技术工程、数学、艺术的跨学科知识，以培养学生的问题解决能力为导向，重点关注学生思维品质的落地生根，全面提高学生基础认知能力与实践能力，促进核心素养的全面发展。
      </p>
      <img
        src="../../../assets/coursesystem/坐标图蓝色@2x.png"
        alt=""
        class="feature"
        @click="preview(2)"
      />
    </div>
    <div class="title">
      <img src="../../../assets/coursesystem/课程-标题4@2x.png" alt="" />
    </div>
    <div class="card">
      <p>
        迪乐姆人工智能课程，为师生提供丰富的教学资源，满足教师与学生的个性化教学需求。
      </p>
      <div class="secend">
        <i></i><span>教学文件：教材、教学设计、课件、学生用书</span>
      </div>
      <div class="secend">
        <i></i
        ><span
          >录播课程：导入视频、解读视频、指导视频、在线课程、双师课堂等。</span
        >
      </div>

      <img
        src="../../../assets/coursesystem/资源 23@2x.png"
        alt=""
        class="feature"
        @click="preview(3)"
      />
    </div>
    <div class="copyright">
      <img src="../../../assets/achievements/底部vi显示备份 3@2x.png" alt="" />
    </div>
  </div>
</template>

<script>
// 使用vant 组件
// import { List, NoticeBar, Cell, Notify } from 'vant'

// 使用装饰器
// import { confirm } from '@/decorator'

// 使用日期工具类
// import { format, DATE_FMT } from '@/utils/date'

// 接口
// import { getDemoData } from '@/api/home'
import { ImagePreview } from 'vant'

export default {
  name: 'Home',
  components: {
    // [List.name]: List,
    // [Cell.name]: Cell,
    // [NoticeBar.name]: NoticeBar
  },
  data() {
    return {
      images: [
        require('../../../assets/coursesystem/特色学校概念图@2x.png'),
        require('../../../assets/coursesystem/课程表@2x.png'),
        require('../../../assets/coursesystem/坐标图蓝色@2x.png'),
        require('../../../assets/coursesystem/资源 @2x.png')
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
  letter-spacing: 1px;

  /** 审查元素，这个样式会转换为 font-size: 4.267vw; */
  //   font-size: 14px;
  background-color: #eaf1f7;
  img {
    width: 100%;
  }
  .title {
    margin: 24px 16px 0 7px;
  }
  .card {
    padding: 14px 14px 8px;
    margin: 18px 16px 0;
    // width: 343px;
    // height: 374px;
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
  }
  .feature {
    margin-top: 20px;
  }
  .copyright {
    margin: 51px 98px;
  }
}
</style>
