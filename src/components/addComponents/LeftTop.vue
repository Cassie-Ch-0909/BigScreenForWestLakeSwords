<template>
  <div id="centerRight1">
    <div class="bg-color-black">
      <div class="d-flex pt-2 pl-2">
        <span>
          <icon name="chart-line" class="text-icon"></icon>
        </span>
        <div class="d-flex">
          <span class="text mx-2">专家委员会</span>
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
        // header: ["姓名", "分支", "覆盖率"],
        data: [
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/8dadced7bad74bd7b7e692957bc6f1d2.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>顾炳中</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国计算机用户协会理事长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;12：00-14：30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;当科幻照进现实我们会更安全吗？</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">做网络安全，既要低头拉车，也要抬头看路</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/8dadced7bad74bd7b7e692957bc6f1d2.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>顾炳中</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国计算机用户协会理事长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;12：00-14：30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;当科幻照进现实我们会更安全吗？</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">做网络安全，既要低头拉车，也要抬头看路</p>
      </div>  
  </div>`,
          ],
        ],
        rowNum: 1, //表格行数
        // headerHeight: 35,
        headerBGC: "#0f1325", //表头
        oddRowBGC: "#0f1325", //奇数行
        evenRowBGC: "#171c33", //偶数行
        // index: true,
        columnWidth: [600],
        // align: ["center"],
        waitTime: 5000,
        carousel: "page",
      },
    };
  },
};
</script>

<style lang="scss" scoped>
$box-height: 410px;
$box-width: 630px;

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
      width: 630px;
      height: 340px;
    }
  }
}
</style>
