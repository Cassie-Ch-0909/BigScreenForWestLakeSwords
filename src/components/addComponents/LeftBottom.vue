<template>
    <div id="centerRight1">
      <div class="bg-color-black">
        <div class="d-flex pt-2 pl-2">
          <span>
            <icon name="chart-line" class="text-icon"></icon>
          </span>
          <div class="d-flex">
            <span class=" text mx-2">大会议程</span>
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
                  <div style="width:950px;height:220px;position:relative">
                <p style="color:#00FFFF;position:absolute;top:-200px;font-size:25px" >5月6日 上午</p>
                <p style="position:absolute;top:-150px;font-size:30px"><span class="colorBlue">会议：</span><span class="colorGrass">95后极客青年Talk</span></p>
                <p style="position:absolute;top:-100px;font-size:20px"><span class="colorBlue">时间：</span><span style="color:white">10：00-10：30</span></p>
                <p style="position:absolute;top:-60px;font-size:20px"><span class="colorBlue">类型：</span><span style="color:white">掌上论剑</p>
                  <p style="position:absolute;top:-20px;font-size:20px"><span class="colorBlue">地点：</span><span style="color:white">线上直播</p>
                
                  <img style="position:absolute;top:40px;width:420px; right:70px;" src="https://img2023.gcsis.cn/2023/5/41cb8e6a1f754988855c3f2e3b278805.png" ></img>
                  </div>`
            ]
            // ['组件1', 'dev-1', "<span  class='colorGrass'>↑75%</span>"],
            // ['组件2', 'dev-2', "<span  class='colorRed'>↓33%</span>"],
            // ['组件3', 'dev-3', "<span  class='colorGrass'>↑100%</span>"],
            // ['组件4', 'rea-1', "<span  class='colorGrass'>↑94%</span>"],
            // ['组件5', 'rea-2', "<span  class='colorGrass'>↑95%</span>"],
            // ['组件6', 'fix-2', "<span  class='colorGrass'>↑63%</span>"],
            // ['组件7', 'fix-4', "<span  class='colorGrass'>↑84%</span>"],
            // ['组件8', 'fix-7', "<span  class='colorRed'>↓46%</span>"],
            // ['组件9', 'dev-2', "<span  class='colorRed'>↓13%</span>"],
            // ['组件10', 'dev-9', "<span  class='colorGrass'>↑76%</span>"]
          ],
          rowNum: 1, //表格行数
          // headerHeight: 90,
          headerBGC: '#0f1325', //表头
          oddRowBGC: '#0f1325', //奇数行
          evenRowBGC: '#171c33', //偶数行
          // index: true,
          // columnWidth: [50],
          align: ['center']
        }
      }
    }
  }
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
  