<template>
  <div class="home">
    <img src="../../../assets/company/公司介绍头图@2x.png" alt="" />

    <div class="title">
      <img src="../../../assets/company/企业简介@2x.png" alt="" />
    </div>

    <div class="card">
      <p>
        迪乐姆（DLM）成⽴于2013年，隶属于上海和盛实业集团有限公司。上海和盛实业集团，是一家产融深度融合的科技产业集团公司，业务涵盖新材料、新能源、教育、AI技术应用、文创消费、大健康等领域。
      </p>
      <p>
        迪乐姆始终围绕创新型人才培训和青少年核心素养提升的教育目标，面向基础教育阶段的中小学、培训机构、学生家庭，提供教育内容研发与教学服务，已为3000所+学校、100000个+家庭提供优质的素质教育服务；举办了500余场教师培训，为学校培养了10000名+优秀的创新教育教师。
      </p>
      <img
        src="../../../assets/company/学校案例4个图标@2x.png"
        alt=""
        class="feature"
      />
      <p>
        自2015年起，迪乐姆成立了创新教育研究院，并在创新教育研究院内设立了研究中⼼、学⽣中⼼、教师中⼼、技术中⼼，致力于以顶层理论研究带动课程研发与师训落地。与中国⼈⼯智能学会、中国⾃动化学会、上海⼈⼯智能技术学会、华东师范⼤学等学术团体、⾼校等达成深度合作，致⼒于打造⼀个合作、共赢、共享的素质教育生态平台。
      </p>
      <p>
        迪乐姆以塑造孩⼦健康⽽优秀的⼈格为使命，以打造国内顶级跨学科素质教育⽣态为愿景⽬标，努⼒为国家素质教育发展做出贡献！
      </p>
      <div class="video">
        <!-- <video width="100%" height="240" controls>
          <source
            src="https://www.runoob.com/try/demo_source/movie.mp4"
            type="video/mp4"
          />
          您的浏览器不支持 HTML5 video 标签。
        </video> -->
        <video-player :options="videoOptions" />
      </div>
    </div>
    <div class="title">
      <img src="../../../assets/company/荣誉证书@2x.png" alt="" />
    </div>
    <div class="card">
      <p>
        自成立以来，迪乐姆一直致力于创新课程的研发和探索，已通过国家高新技术企业认证、ISO9001质量管理体系认证；成为中国教育装备理事单位、中国自动化学会青少年人工智能核心素养测评联合发起单位。
      </p>
      <img
        src="../../../assets/company/8个荣誉证书@2x.png"
        alt=""
        class="feature"
      />
    </div>

    <div class="title">
      <img src="../../../assets/company/专利证书@2x.png" alt="" />
    </div>
    <div class="card">
      <p>
        迪乐姆注重自主知识产权研发，现已获得作品著作权577个、软件著作权47个、商标产权33个、专利32个。
      </p>
      <img
        src="../../../assets/company/9个专利证书@2x.png"
        alt=""
        class="feature"
      />
    </div>

    <div class="copyright">
      <img src="../../../assets/achievements/底部vi显示备份 3@2x.png" alt="" />
    </div>
  </div>
</template>

<script>
// 使用vant 组件
import VideoPlayer from '@/components/VideoPlayer.vue'

export default {
  name: 'Home',
  components: {
    VideoPlayer
  },
  data() {
    return {
      videoOptions: {
        autoplay: false,
        controls: true,
        height: 200,
        poster: require('../../../assets/company/video.png'),
        sources: [
          {
            src: 'https://teacher.delightmom.com/wx/video/dlm.mp4',
            type: 'video/mp4'
          }
        ]
      }
    }
  }
}
</script>
<style lang="less" scoped>
.home {
  /** 审查元素，这个样式会转换为 font-size: 4.267vw; */
  //   font-size: 14px;
  background-color: #eaf1f7;
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
    width: 136px;
    margin-top: 4px;
    margin-bottom: 14px;
  }
  .xueshu3 {
    width: 96px;
    margin-top: 4px;
    margin-bottom: 14px;
  }
  .xueshu4 {
    width: 84px;
    margin-top: 4px;
    margin-bottom: 14px;
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
