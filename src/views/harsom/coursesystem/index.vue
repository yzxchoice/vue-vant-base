<template>
  <div class="home">
    <img src="../../../assets/coursesystem/coursehead.png" alt="" />
    <div class="title">
      <img src="../../../assets/coursesystem/title1.png" alt="" />
    </div>

    <div class="card">
      <p>
        迪乐姆人工智能课程以点、线、面多维途径展开，满足基础普适、兴趣拓展、竞赛提升不同场景的教学需求，为处于不同年龄、不同基础、不同目标的学生人群打造系统的课程体系，完美融合现有教育生态。
      </p>
      <img
        src="../../../assets/coursesystem/feature.png"
        alt=""
        class="feature"
      />
    </div>
    <div class="title">
      <img src="../../../assets/coursesystem/title2.png" alt="" />
    </div>
    <div class="card">
      <p>
        迪乐姆人工智能课程，以信息科技课程标准为依据，符合育人为先，科学原理与实践应用并重，鼓励“做中学”、“用中学”、“创中学”的课程要求，是学校课程的有效补充。
      </p>
      <img
        src="../../../assets/coursesystem/classlist.png"
        alt=""
        class="feature"
      />
    </div>
    <div class="title">
      <img src="../../../assets/coursesystem/title3.png" alt="" />
    </div>
    <div class="card">
      <p>
        迪乐姆人工智能课程，以TPI课程建构理论为依据，融合科学、技术工程、数学、艺术的跨学科知识，以培养学生的问题解决能力为导向，重点关注学生思维品质的落地生根，全面提高学生基础认知能力与实践能力，促进核心素养的全面发展。
      </p>
      <img
        src="../../../assets/coursesystem/coordinate.png"
        alt=""
        class="feature"
      />
    </div>
    <div class="title">
      <img src="../../../assets/coursesystem/title4.png" alt="" />
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
        src="../../../assets/coursesystem/resource.png"
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
// import { List, NoticeBar, Cell, Notify } from 'vant'

// 使用装饰器
// import { confirm } from '@/decorator'

// 使用日期工具类
// import { format, DATE_FMT } from '@/utils/date'

// 接口
// import { getDemoData } from '@/api/home'

export default {
  name: 'Home',
  components: {
    // [List.name]: List,
    // [Cell.name]: Cell,
    // [NoticeBar.name]: NoticeBar
  },
  data() {
    return {
      //   currentDate: format(new Date(), DATE_FMT)
    }
  },
  created() {},

  methods: {
    // @confirm('这是通过装饰器添加的确认信息', '提示')
    // $_handleUseDecorator() {
    //   console.log(`
    //             你还可以使用
    //             @alert 提示框
    //             @throttle 函数节流
    //             @debounce 函数防抖
    //             更多装饰器正在完善中
    //           `)
    // },
    // // 加载数据
    // async $_loadData() {
    //   const loading = this.$loading()
    //   try {
    //     console.log(await getDemoData())
    //     Notify({
    //       message: '数据加载成功',
    //       type: 'success'
    //     })
    //   } catch (error) {
    //     console.error(error)
    //   } finally {
    //     loading.close()
    //   }
    // },
    // goJump() {
    //   this.$router.push({ name: 'TestAbout' })
    // }
  }
}
</script>
<style lang="less" scoped>
.home {
  /** 审查元素，这个样式会转换为 font-size: 4.267vw; */
  //   font-size: 14px;
  background-color: #eaf1f7;
  letter-spacing: 1px;
  img {
    width: 100%;
  }
  .title {
    margin: 24px 16px 0 7px;
  }
  .card {
    margin: 18px 16px 0;
    // width: 343px;
    // height: 374px;
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
    margin-top: 20px;
  }
  .copyright {
    margin: 51px 98px;
  }
}
</style>
