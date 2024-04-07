<template>
  <div id="centerRight1">
    <div class="bg-color-black">
      <div class="d-flex pt-2 pl-2">
        <span>
          <i class="iconfont icon-chengguofabu colorBlue" style="font-size: 20px; padding-bottom:10px;"></i>
          <!-- <icon name="chart-line" class="text-icon"></icon> -->
        </span>
        <div class="d-flex">
          <span class="text mx-2">成果发布</span>
        </div>
      </div>
      <div class="d-flex jc-center body-box">
        <dv-scroll-board class="dv-scr-board" :config="config" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      config: {
        // header: ['组件', '分支', '覆盖率'],
        data: [
          [
            `
            <div style="width:560px; height:450px; position:relative;">
              <img style="width:190px;position:absolute;top:10px;left:5px" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/7/70fe3218d7ae4f58ae91a838ed4d64dd.jpg"></img>
              <p style="color:white;position:absolute;left:250px;top:-150px;font-size:30px" class="colorBlue">2023西湖论剑 ----</p>
              <p style="color:white;position:absolute;left:250px;top:-100px;font-size:30px" class="colorBlue">11周年精华特刊</p>
              <p style="color:white;position:absolute;left:0px;top:0px;font-size:20px">建没数宇中国是我国的重要国策。在《数宇中国建设整体</p>
              <p style="color:white;position:absolute;left:0px;top:30px;font-size:20px">布局规划〉 (以下简称《规划》)中明确了数字中国建设按</p>
              <p style="color:white;position:absolute;left:0px;top:60px;font-size:20px">照“2522”的整体框架进行布局。整体框架中，一方面着重</p>
              <p style="color:white;position:absolute;left:0px;top:90px;font-size:20px">强调了数字安全的重要性，数字安全和数字技术并列为支</p>
              <p style="color:white;position:absolute;left:0px;top:120px;font-size:20px">撑数字中国建设的两大能力。另一方面，“安全”在2522框</p>
              <p style="color:white;position:absolute;left:0px;top:150px;font-size:20px">架中无处不在——数字基础设施不可无安全保障，数据资</p>
              <p style="color:white;position:absolute;left:0px;top:180px;font-size:20px">源大循环不可无安全赋能，建设公平规范的数字治理生态</p>
              <p style="color:white;position:absolute;left:0px;top:210px;font-size:20px">不可无安全辅助。建设数字中国势在必行。</p>
              </div>
            `
          ],
          [
            `
            <div style="width:560px; height:450px; position:relative;">
              <img style="width:150px;position:absolute;top:10px;left:5px" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/5/8cc23042ae8f4a6e80f25997132d13c0.png"></img>
              <p style="color:white;position:absolute;left:250px;top:-150px;font-size:30px" class="colorBlue">2023数字安全能力</p>
              <p style="color:white;position:absolute;left:250px;top:-100px;font-size:30px" class="colorBlue">洞察报告</p>
              <p style="color:white;position:absolute;left:0px;top:10px;font-size:20px">数字经济成为全球新一轮科技革命和产业变革的重要引擎，</p>
              <p style="color:white;position:absolute;left:0px;top:40px;font-size:20px">将开启人类数字文明的新时代。数字安全的基础性作用日</p>
              <p style="color:white;position:absolute;left:0px;top:70px;font-size:20px">益突出，在数字化建设进程中，加紧实施国家信息化发展</p>
              <p style="color:white;position:absolute;left:0px;top:100px;font-size:20px">战略，筑牢可信可控的数字安全屏障，夯实数字基础设施</p>
              <p style="color:white;position:absolute;left:0px;top:130px;font-size:20px">安全底座，增强关键基础设施安全韧性，助力数字社会安</p>
              <p style="color:white;position:absolute;left:0px;top:160px;font-size:20px">全发展，已成为支撑现代化建设、增强国家综合实力的必</p>
              <p style="color:white;position:absolute;left:0px;top:190px;font-size:20px">然选择。</p>
              </div>
            `
          ],
          [
            `
            <div style="width:560px; height:450px; position:relative;">
              <img style="width:210px;position:absolute;top:40px;left:5px" src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/5/0bfbde79d1774b43bab8f03d1c75e44c.png"></img>
              <p style="color:white;position:absolute;left:240px;top:-170px;font-size:30px" class="colorBlue">安恒信息2023年</p>
              <p style="color:white;position:absolute;left:240px;top:-130px;font-size:30px" class="colorBlue">行业解决方案蓝皮书</p>
              <p style="color:white;position:absolute;left:220px;top:-90px;font-size:30px">（全6本）</p>
              <p style="color:white;position:absolute;left:0px;top:10px;font-size:20px">数字安全是未来数字化发展的重要组成部分，立足数字安</p>
              <p style="color:white;position:absolute;left:0px;top:40px;font-size:20px">全建设。备预不虞，为国常道，安恒信息结合多年网络安</p>
              <p style="color:white;position:absolute;left:0px;top:70px;font-size:20px">全、数据安全经验以及对行业发展趋势的理解和把握，安</p>
              <p style="color:white;position:absolute;left:0px;top:100px;font-size:20px">恒信息首次发布六大行业解决方案蓝皮书，全面介绍网信</p>
              <p style="color:white;position:absolute;left:0px;top:130px;font-size:20px">、公安、运营商、金融、教育、交通六大行业中的解决方</p>
              <p style="color:white;position:absolute;left:0px;top:160px;font-size:20px">案最佳实践，为产业数字化发展指明了方向，全面加速推</p>
              <p style="color:white;position:absolute;left:0px;top:190px;font-size:20px">动经济社会全面发展。</p>
              </div>
            `
          ],
          [
            `
            <div style="width:560px; height:450px; position:relative;">
              <img style="width:210px;height:160px;position:absolute;top:40px;left:5px" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/5/bf77ef3740464bd38b383633d30831a6.jpg"></img>
              <p style="color:white;position:absolute;left:240px;top:-130px;font-size:30px" class="colorBlue">下一代防火墙</p>
              <p style="color:white;position:absolute;left:0px;top:10px;font-size:20px">明御防火墙（DAS-TGFW）秉持“持续边界安全态势改善”</p>
              <p style="color:white;position:absolute;left:0px;top:40px;font-size:20px">的理念，以用户为核心，以边界、应用、威胁、权限为防</p>
              <p style="color:white;position:absolute;left:0px;top:70px;font-size:20px">护对象，构建了以资产为视角的可持续智能安全运营防护</p>
              <p style="color:white;position:absolute;left:0px;top:100px;font-size:20px">体系。是集传统防火墙、入侵防御、防病毒、上网行为管</p>
              <p style="color:white;position:absolute;left:0px;top:130px;font-size:20px">控、VPN、威胁情报等安全模块于一身，同时可联合态势</p>
              <p style="color:white;position:absolute;left:0px;top:160px;font-size:20px">感知、EDR等产品进行一体化建设的智能安全网关。</p>
              </div>
            `
          ],
          [
            `
            <div style="width:560px; height:450px; position:relative;">
              <img style="width:210px;height:160px;position:absolute;top:40px;left:5px" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/5/500e36be359f492ab623b7998263ccc2.jpg"></img>
              <p style="color:white;position:absolute;left:240px;top:-170px;font-size:30px" class="colorBlue">安全托管运营服务</p>
              <p style="color:white;position:absolute;left:240px;top:-130px;font-size:30px" class="colorBlue">MSS</p>
              <p style="color:white;position:absolute;left:0px;top:10px;font-size:20px">提供体系化、常态化的安全托管服务，协助构建7*24小时</p>
              <p style="color:white;position:absolute;left:0px;top:40px;font-size:20px">全天候、全方位的安全运营体系， 实现安全风险从发现到</p>
              <p style="color:white;position:absolute;left:0px;top:70px;font-size:20px">响应处置的闭环，持续不断提高网络安全水平</p>
              </div>
            `
          ],
          [
            `
            <div style="width:560px; height:450px; position:relative;">
              <img style="width:210px;position:absolute;top:10px;left:5px" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/cd902015f99246108a0615d4668f5d0d.png"></img>
              <p style="color:white;position:absolute;left:220px;top:-150px;font-size:30px" class="colorBlue">数据安全与隐私计算</p>
              <p style="color:white;position:absolute;left:0px;top:0px;font-size:20px">本书首先介绍了业内多个具备代表性的数据安全理论及实</p>
              <p style="color:white;position:absolute;left:0px;top:30px;font-size:20px">践框架，从数 据常见风险出发，引出数据安全保护最佳实</p>
              <p style="color:white;position:absolute;left:0px;top:60px;font-size:20px">践，然后介绍了数字经济时代数据要素市场的基本信息，</p>
              <p style="color:white;position:absolute;left:0px;top:90px;font-size:20px">基于构建数据要素市场、促进数据合规安全流通，释放数</p>            
              <p style="color:white;position:absolute;left:0px;top:120px;font-size:20px">据价值等场景中的实践，抽象并总结了一套数据要素可信、</p>              
              <p style="color:white;position:absolute;left:0px;top:150px;font-size:20px">安全、合 规流通的体系架构，包括数据安全保护技术与保</p>              
              <p style="color:white;position:absolute;left:0px;top:180px;font-size:20px">护数据价值释放的隐私计算 技术，最后针对政务、金融、</p>              
              <p style="color:white;position:absolute;left:0px;top:210px;font-size:20px">电力能源、公安行业等重点行业，分析了数据 安全与数...</p>            
              </div>
            `,
          ],
        ],
        rowNum: 1, //表格行数
        // headerHeight: 35,
        headerBGC: "#0f1325", //表头
        oddRowBGC: "#0f1325", //奇数行
        evenRowBGC: "#171c33", //偶数行
        // index: true,
        // columnWidth: [100,100,170],
        align: ["center"],
        waitTime: 5000,
        carousel: "page",
      },
    };
  },
};
</script>

<style lang="scss" scoped>
$box-height: 460px;
$box-width: 560px;
#centerRight1 {
  padding: 16px;
  padding-top: 20px;
  height: $box-height;
  width: $box-width;
  border-radius: 5px;
  .bg-color-black {
    height: $box-height - 30px;
    border-radius: 10px;
  }
  .text {
    color: #c3cbde;
  }
  .body-box {
    border-radius: 10px;
    overflow: hidden;
    .dv-scr-board {
      width: 560px;
      height: 455px;
    }
  }
}
</style>
