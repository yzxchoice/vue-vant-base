<template>
  <div class="home">
    <img src="../../../assets/case/成功案例头图@2x.png" alt="" />

    <div class="title">
      <img src="../../../assets/case/校园案例@2x.png" alt="" />
    </div>

    <div class="card">
      <p>
        迪乐姆针对幼教、普教的创新教育场景，以提升学⽣不同阶段的创新素养为⽬标，⽤专业的课程、完善的服务，推动学校素质教育发展，为国家培养创新型⼈才做贡献。截止到2021年，迪乐姆已为3000多所学校、100000多个家庭提供优质的素质教育服务。
      </p>
      <img src="../../../assets/case/4个图标@2x.png" alt="" class="feature" />

      <div class="titleimg">
        <img src="../../../assets/case/编组 5@2x.png" alt="" />
      </div>
      <p>立足上海，辐射全国，用户遍及20余个省市</p>
      <img src="../../../assets/case/案例地图@2x.png" alt="" class="feature" />
    </div>
    <div class="title">
      <img src="../../../assets/case/案例名单@2x.png" alt="" />
    </div>
    <van-tabs v-model="active">
      <van-tab title="华东区">
        <div class="casecard">
          <div class="header">上海</div>
          <div
            v-for="(item, index) in shanghai"
            :key="'shanghai' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">浙江</div>
          <div
            v-for="(item, index) in zhejiang"
            :key="'zhejiang' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">江苏</div>
          <div
            v-for="(item, index) in jiangsu"
            :key="'jiangsu' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">安徽</div>
          <div
            v-for="(item, index) in anhui"
            :key="'anhui' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">江西</div>
          <div
            v-for="(item, index) in jiangxi"
            :key="'jiangxi' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">山东</div>
          <div
            v-for="(item, index) in shandong"
            :key="'shandong' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">福建</div>
          <div
            v-for="(item, index) in fujian"
            :key="'fujian' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab>
      <van-tab title="华北区">
        <div class="casecard">
          <div class="header">内蒙古</div>
          <div
            v-for="(item, index) in neimenggu"
            :key="'neimenggu' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">山西</div>
          <div
            v-for="(item, index) in shanxi"
            :key="'shanxi' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">河北</div>
          <div
            v-for="(item, index) in hebei"
            :key="'hebei' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab>
      <van-tab title="华中区">
        <div class="casecard">
          <div class="header">河南</div>
          <div
            v-for="(item, index) in henan"
            :key="'henan' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">湖南</div>
          <div
            v-for="(item, index) in hunan"
            :key="'hunan' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">湖北</div>
          <div
            v-for="(item, index) in hubei"
            :key="'hubei' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab>
      <van-tab title="西北区">
        <div class="casecard">
          <div class="header">宁夏</div>
          <div
            v-for="(item, index) in ningxia"
            :key="'ningxia' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">甘肃</div>
          <div
            v-for="(item, index) in gansu"
            :key="'gansu' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">新疆</div>
          <div
            v-for="(item, index) in xinjiang"
            :key="'xinjiang' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">陕西</div>
          <div
            v-for="(item, index) in shanerxi"
            :key="'shanerxi' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab>
      <van-tab title="西南区">
        <div class="casecard">
          <div class="header">贵州</div>
          <div
            v-for="(item, index) in guizhou"
            :key="'guizhou' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">四川</div>
          <div
            v-for="(item, index) in sichuan"
            :key="'sichuan' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">重庆</div>
          <div
            v-for="(item, index) in chongqing"
            :key="'chongqing' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">云南</div>
          <div
            v-for="(item, index) in yunnan"
            :key="'yunnan' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">西 藏</div>
          <div
            v-for="(item, index) in xizang"
            :key="'xizang' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">广 西</div>
          <div
            v-for="(item, index) in guangxi"
            :key="'guangxi' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab>
      <van-tab title="东北区">
        <div class="casecard">
          <div class="header">吉林</div>
          <div
            v-for="(item, index) in jilin"
            :key="'jilin' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">黑龙江</div>
          <div
            v-for="(item, index) in heilongjiang"
            :key="'heilongjiang' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
          <div class="header">辽 宁</div>
          <div
            v-for="(item, index) in liaoning"
            :key="'liaoning' + index"
            class="item"
          >
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab>
      <!-- <van-tab title="其他">
        <div class="casecard">
          <div class="header">其他</div>
          <div v-for="(item, index) in qita" :key="'qita' + index" class="item">
            <i></i>
            <span>{{ item }}</span>
          </div>
        </div>
      </van-tab> -->
    </van-tabs>

    <div class="title">
      <img src="../../../assets/case/案例展示@2x.png" alt="" />
    </div>
    <div class="title casetext">
      <img src="../../../assets/case/一站式文字备份@2x.png" alt="" />
    </div>
    <div>
      <van-swipe class="my-swipe" :loop="false" :width="320" :height="300">
        <van-swipe-item>
          <img src="../../../assets/case/编组 41@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/case/编组 41备份@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/case/编组 41备份 2@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/case/编组 41备份 4@2x.png" alt="" />
        </van-swipe-item>
        <van-swipe-item>
          <img src="../../../assets/case/编组 41备份 5@2x.png" alt="" />
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
import { Tab, Tabs, Swipe, SwipeItem } from 'vant'

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
      active: 0,
      shanghai: [
        '上海市长岛中学',
        '上海市黄浦区市南中学',
        '上海市黄浦区敬业中学上海市长岛中学',
        '上海市黄浦区市南中学',
        '上海市黄浦区敬业中学新民小学',
        '横沙小学',
        '崇明实验小学',
        '江口小学',
        '登瀛小学',
        '竖新小学',
        '港沿小学',
        '合兴小学',
        '长兴小学',
        '东门小学'
      ],
      zhejiang: [
        '绍兴东湖中学',
        '诸暨荣怀学校',
        '秋滨小学',
        '许村镇许巷中心小学',
        '绍兴聋哑学校',
        '永康外国语学校',
        '浙江东湖小学',
        '浙江绍兴秋瑾小学',
        '龙游小南海小学'
      ],
      jiangsu: [
        '江苏省睢宁高级中学',
        '苏州市教育科学研究院附属实验学校',
        '苏州市南环实验学校',
        '南通市天生港小学'
      ],
      anhui: [
        '宁国开发区实验小学',
        '合肥一六八玫瑰园中学',
        '砀山县第六中学',
        '砀山县西关小学',
        '砀山县第三小学',
        '砀山县李庄中学',
        '砀山县文庄中学',
        '砀山县程庄中学',
        '阜阳市第二中学',
        '阜阳市第十九中学',
        '阜阳市实验小学',
        '合肥高新区创新实验第二小学',
        '长丰县中心小学',
        '滁州外国语学校附属苏滁实验中学'
      ],
      jiangxi: [
        '江西工程学院学前教育实训室',
        '瑞昌市第五小学',
        '德兴市铜都中学',
        '廉溪区第二小学',
        '濂溪区浔南小学'
      ],
      shandong: [
        '沂水县第四中学',
        '山东日照二中',
        '古柳小学',
        '盛隆小学',
        '亚沙城小学',
        '新元小学'
      ],
      fujian: [
        '宁德市东侨经济技术开发区中学',
        '古田县教育局小学',
        '福建省三明第一中学',
        '福州大学'
      ],
      neimenggu: [
        '锡盟正蓝旗教育局',
        '呼伦贝尔市陈巴尔虎旗小学',
        '呼伦贝尔市陈巴尔虎旗中学',
        '兴安盟卫东镇政府'
      ],
      shanxi: [
        '太原市青年路小学分校',
        '临汾市解放路小学',
        '五寨县职业中学',
        '乡宁县幸福湾小学',
        '天镇县第一小学',
        '泽州县枣园学校',
        '灵丘县第一中学',
        '代县教育局',
        '怀仁市第二实验小学'
      ],
      henan: [
        '南乐县第一高级中学',
        '河南师范大学',
        '信阳市浉河中学',
        '郑州市毓秀路实验小学',
        '固始县第十三小学',
        '林州市第一中学',
        '信阳师范学院教科院'
      ],
      hunan: [
        '湖南怀化铁路第一中学',
        '浏阳新屋里小学',
        '永州市冷水滩区青少年活动中心',
        '郴州幼儿园'
      ],
      hubei: [
        '大冶市第二中学',
        '武汉市崇文外国语学校',
        '汉川福星中学、马口敖家小学',
        '浠水科技馆'
      ],
      ningxia: [
        '中卫第七中学',
        '海原县第二中学',
        '泾源县兴盛小学',
        '石嘴山市第十五小学',
        '灵武市第五中学',
        '固原五中',
        '银川市兴庆区教育局第二十五小学',
        '石嘴山市第七中学',
        '石嘴山市第六中学',
        '石嘴山第二十小学',
        '银川唐徕回民中学西校区',
        '银川回民中学',
        '固原一中',
        '石嘴山隆湖一站学校',
        '石嘴山市第八中学'
      ],
      gansu: [
        '泾川东街小学',
        '兰州市碧桂园学校',
        '天水市麦积区天润学校',
        '平凉一中新校区',
        '宁县宁江小学'
      ],
      xinjiang: [
        '哈密市第三中学',
        '库尔勒市第二小学',
        '玛纳斯县小学',
        '新疆阜康创客实验室',
        '和硕县第二中学',
        '克拉玛依第六中学'
      ],
      shanerxi: [
        '太白县幼儿园',
        '商南县第八小学',
        '西安高新区第十七小学',
        '渭南市临渭区青少年校外活动中心',
        '灞桥区第六十三中学',
        '略阳县徐家坪初级中学',
        '蓝田创客中心',
        '西安市长安区郭杜街道中心学校',
        '周至县新区小学',
        '西安航天城第三小学',
        '沣西中学',
        '西安高新区第十四小学',
        '陕西师范大学林凯城小学',
        '神木市第三中学',
        '子长市中学',
        '金茂府小学',
        '延安市深沟希望小学',
        '孔家庄小学',
        '西安高新第九中学',
        '陕西师范大学杨凌实验中学',
        '高新区第十三小学',
        '渭柳佳苑中学',
        '高新区第十六小学',
        '恒大二小',
        '长安三小项目',
        '西安惠安小学',
        '西安高新区第十四小学',
        '师大附小嘉园小学',
        '西北大学幼儿园',
        '陕西师范大学国际商学院',
        '碧桂园凤凰城小学、中学',
        '高新区第八小学',
        '子长市中学',
        '西安市第三十中学'
      ],
      guizhou: [
        '罗甸边阳中学',
        '德江县教育局',
        '镇远县城关五小',
        '金堡镇中心小学',
        '六盘水第四中学',
        '贵阳市第三实验中学',
        '贵州大方第七中学',
        '贵州文德金堡小学',
        '遵义市播州区教育设施设备'
      ],
      sichuan: [
        '会东县会东中学',
        '会东县职业技术学院',
        '会东县和文中学',
        '乐山东辰国际学校',
        '广元市利州区三堆小学',
        '广元市利州区宝轮镇七一小学',
        '广元市利州区宝轮第一小学',
        '四川仪陇宏德中学',
        '四川省教科院附属中学'
      ],
      chongqing: [
        '重庆市九龙坡区谢家湾学校初中部',
        '重庆聋哑学校',
        '重庆新华小学',
        '重庆市綦江区青康德城小学'
      ],
      yunnan: [
        '芒令小学',
        '个旧大屯小学',
        '五华区云铜小学',
        '官渡区东站实验学校',
        '昆明市呈贡区斗南学校',
        '高新一小附属磊鑫外国语学校',
        '昆明市盘龙区东华小学'
      ],
      jilin: [
        '长春国际物流经济开发区实验学校',
        '东北师大附属中学深圳学校',
        '长春市华蕴学校'
      ],
      qita: [
        '邯郸市荀子小学',
        '广西乡村学校少年宫',
        '锦州市现代服务学校',
        '林芝市第一中学',
        '拉萨市北京中学',
        '虎林职业高中',
        '鸡西市虎林第五小学'
      ],
      hebei: ['邯郸市荀子小学'],
      heilongjiang: ['鸡西市虎林第五小学', '虎林职业高中'],
      liaoning: ['锦州市现代服务学校'],
      xizang: ['林芝市第一中学', '拉萨市北京中学'],
      guangxi: ['邯郸市荀子小学']
    }
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
  .my-swipe {
    margin: 10px 0 10px 16px;
  }
  .my-swipe .van-swipe-item {
    font-size: 20px;
    line-height: 150px;
    color: #ffffff;
    text-align: center;
    img {
      width: 90%;
    }
  }
  // .custom-indicator {
  //   position: absolute;
  //   right: 5px;
  //   bottom: 5px;
  //   padding: 2px 5px;
  //   font-size: 12px;
  //   background: rgba(0, 0, 0, 0.1);
  // }
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
    .titleimg {
      width: 99px;
      height: 25px;
      margin: 30px 0 7px;
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
  .casetext {
    width: 252px;
    height: 65px;
    margin-left: 16px;
  }
  .feature {
    margin-top: 18px;
    margin-bottom: 29px;
  }
  .copyright {
    margin: 51px 98px;
  }

  .casecard {
    margin-top: 12px;
    font-size: 14px;
    font-weight: 500;
    color: #303232;
    background: #ffffff;
    border-radius: 10px;
    box-shadow: 4px 4px 6px 0 rgba(115, 140, 187, 0.32);

    .header {
      height: 48px;
      line-height: 48px;
      text-align: center;
      background-color: #f3f7fb;
      &:nth-child(1) {
        border-radius: 8px;
      }
    }
    .item {
      display: flex;
      align-items: center;
      padding: 18px 14px 14px 23px;
      border-bottom: 1px solid #eaf1f7;
      i {
        display: inline-block;
        width: 5px;
        height: 5px;
        margin-right: 8px;
        background-color: #2b71fa;
        border-radius: 50%;
      }
    }
  }
}
</style>
