<template>
  <div id="centerRight1">
    <div class="bg-color-black">
      <div class="d-flex pt-2 pl-2">
        <span>
          <icon name="chart-line" class="text-icon"></icon>
        </span>
        <div class="d-flex">
          <span class=" text mx-2">展商风采</span>
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
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d79ec14ff65b4af19b8439659668fd19.png"></img>`,
            "宝德",
            "PowerLeader",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d86aad180ee14acb95d1df723414aec2.png"></img>`,
            "乐研科技",
            `<span class="colorGrass">RYALTECH</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d79ec14ff65b4af19b8439659668fd19.png"></img>`,
            "宝德",
            "PowerLeader",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d86aad180ee14acb95d1df723414aec2.png"></img>`,
            "乐研科技",
            `<span class="colorGrass">RYALTECH</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d79ec14ff65b4af19b8439659668fd19.png"></img>`,
            "宝德",
            "PowerLeader",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d86aad180ee14acb95d1df723414aec2.png"></img>`,
            "乐研科技",
            `<span class="colorGrass">RYALTECH</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d79ec14ff65b4af19b8439659668fd19.png"></img>`,
            "宝德",
            "PowerLeader",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d86aad180ee14acb95d1df723414aec2.png"></img>`,
            "乐研科技",
            `<span class="colorGrass">RYALTECH</span>`,
          ],
        ],
        rowNum: 5, //表格行数
        // headerHeight: 35,
        headerBGC: '#0f1325', //表头
        oddRowBGC: '#0f1325', //奇数行
        evenRowBGC: '#171c33', //偶数行
        // index: true,
        columnWidth: [100,100,170],
        align: ['center']
      }
    }
  }
}
</script>

<style lang="scss" scoped>
$box-height: 455px;
$box-width: 375px;
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
      width: 375px;
      height: 455px;
    }
  }
}
</style>