<template>
  <div id="centerRight1">
    <div class="bg-color-black">
      <div class="d-flex pt-2 pl-2">
        <span>
          <i class="iconfont icon-dahuiyicheng colorBlue"></i>
          <!-- <icon name="chart-line" class="text-icon" style="background-color: aqua;"></icon> -->
        </span>
        <div class="d-flex">
          <span class="text mx-2">大会议程</span>
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
            `<div style="width:950px;height:220px;position:relative">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月5日下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">格致论道@西湖论剑</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">18：00-21：00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">科普论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州市滨江区文化中心剧院一层</p>

                <img style="position:absolute;top:40px;width:420px; right:70px;" src="https://img2023.gcsis.cn/2023/4/62eaf1128543498d87fefbe31913a5a3.jpeg" ></img>
                </div>
                <div style="width:950px;height:220px;margin-top:10px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月6日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">95后极客青年Talk</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">10：00-10：30</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">掌上论剑</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:40px;width:420px; right:70px;" src="https://img2023.gcsis.cn/2023/5/41cb8e6a1f754988855c3f2e3b278805.png" ></img>
                </div>`,
          ],
          [
            `<div style="width:950px;height:220px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月6日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">当科幻照进现实我们会更安全吗？</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:00 - 13:30</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">掌上论剑</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/41cb8e6a1f754988855c3f2e3b278805.png" ></img>
                </div>
                <div style="width:950px;height:220px;position:relative">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月6日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">人工智能会颠覆安全行业吗？</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">15:00 - 15:30</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">掌上论剑</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/5b42164afc34441ead239085ffd3c657.png" ></img>
                </div>`,
          ],
          [
            `<div style="width:950px;height:220px;position:relative;">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月6日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">反诈直播间@西湖论剑</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">15:30 - 16:30</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">掌上论剑</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/effacedd0d444862b56ff2cbc526e5b4.jpg" ></img>
                </div>
                <div style="width:950px;height:220px;margin-top:10px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月7日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">主论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">09:00 - 12:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">主论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·杭州厅</p>

                <img style="position:absolute;top:30px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/4/fe482a3064d94335b98fa35fab1ed755.jpg" ></img>
                </div>`,
          ],
          [
            `<div style="width:950px;height:220px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月7日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">生态合作伙伴分论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">09:00 - 22:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">生态合作</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州英冠索菲特酒店</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://2023.gcsis.cn/uploadfile/7329eddebec94200a74a2e9a9753f9c3.jpg" ></img>
                </div>
                <div style="width:950px;height:220px;position:relative">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月6日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">数字中国&安全治理论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:30 - 18:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">主论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·杭州厅</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/dc6fdbc88cca4305be2e11797da43d06.jpg" ></img>
                </div>`,
          ],
          [
            `<div style="width:950px;height:220px;position:relative;">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月6日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">信创软件供应链安全论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:30 - 17:10</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·天津厅</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/9311c97475fc495999aecdb672038492.jpeg" ></img>
                </div>
                <div style="width:950px;height:220px;margin-top:10px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月7日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">车联网安全论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:30 - 17:30</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·北京厅</p>

                <img style="position:absolute;top:30px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/6/6d177be629c84594b0a86c5d0b8eb15a.jpeg" ></img>
                </div>`,
          ],
          [
            `<div style="width:950px;height:220px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月7日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">工业领域网络和数据安全论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:30 - 17:30</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·北京厅</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/d3d77cc2536040daa2325c5b5a1d1e8c.jpeg" ></img>
                </div>
                <div style="width:950px;height:220px;position:relative">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月7日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">网络安全创新发展高端论坛（无回放）</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:30 - 17:40</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·国际厅2厅</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/4/8ac152e8260c4ed98e35c9756272dddb.jpeg" ></img>
                </div>`,
          ],
          [
            `<div style="width:950px;height:220px;position:relative;">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月7日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">第二直播间</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">09:30 - 12:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">第二直播间</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/45d149bf8b5245a9802d35d7c299033f.jpeg" ></img>
                </div>
                <div style="width:950px;height:220px;margin-top:10px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月8日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">教育技术产业融合创新发展论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white"> 08:30 - 12:10</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white"> 平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·国际厅1厅</p>

                <img style="position:absolute;top:30px;width:340px; right:70px;" src="	https://img2023.gcsis.cn/2023/5/3692fcd308d94db8b345f06d65a2b278.jpg" ></img>
                </div>`,
          ],

          [
            `<div style="width:950px;height:220px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月8日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">商用密码应用论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">09:00 - 12:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·北京厅</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/4/4e2a3ecef60540aaad44363e3c70a12a.jpeg" ></img>
                </div>
                <div style="width:950px;height:220px;position:relative">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月8日 上午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">第二直播间</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white"> 09:30 - 12:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">第二直播间</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/45d149bf8b5245a9802d35d7c299033f.jpeg" ></img>
                </div>`,
          ],

          [
            `<div style="width:950px;height:220px;position:relative;">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" class="colorGreen">5月8日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">MSS安全托管运营服务论坛</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">13:30 - 18:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">平行论坛</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">杭州洲际酒店·国际厅1厅</p>

                <img style="position:absolute;top:15px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/933ffa78bfad4121a1b763c6beb9f11d.jpeg" ></img>
                </div>
                <div style="width:950px;height:220px;margin-top:10px;position:relative;background-color:rgba(0,0,0,0.5)">
              <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月8日 下午</p>
              <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">生态“朋友圈”</span></p>
              <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">12:30 - 13:00</span></p>
              <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white"> 第二直播间</p>
                <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>

                <img style="position:absolute;top:30px;width:340px; right:70px;" src="https://img2023.gcsis.cn/2023/5/d4e40b2d7f514810967e7efb9eadb77c.jpg" ></img>
                </div>`,
          ],
        ],
        rowNum: 1, //表格行数
        // headerHeight: 90,
        headerBGC: "#0f1325", //表头
        oddRowBGC: "#0f1325", //奇数行
        evenRowBGC: "#171c33", //偶数行
        // index: true,
        // columnWidth: [50],
        align: ["center"],
        carousel:'page',
        waitTime:5000
      },
    };
  },
};
</script>

<style lang="scss" scoped>
$box-height: 520px;
$box-width: 950px;
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
      padding-top: 10px;
      width: 900px;
      height: 455px;
    }
  }
}
</style>
