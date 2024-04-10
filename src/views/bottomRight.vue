<template>
  <div id="centerRight1">
    <div class="bg-color-black">
      <div class="d-flex pt-2 pl-2">
        <span>
          <i
            class="iconfont icon-fengcai colorBlue"
            style="font-size: 20px"
          ></i>
          <!-- <icon name="chart-line" class="text-icon"></icon> -->
        </span>
        <div class="d-flex">
          <span class="text mx-2">展商风采</span>
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
            "宝德计算",
            "PowerLeader",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/d86aad180ee14acb95d1df723414aec2.png"></img>`,
            "乐研科技",
            `<span class="colorGrass">RYALTECH</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/8077d0d14baa4eb9ad78181285b0ee09.png"></img>`,
            "上元信安",
            "SUNYANFO",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/2cf78591048d49d28414ee2b1426d4f9.png"></img>`,
            "中尔网络",
            `<span class="colorGrass">Network Techology</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/73bd035a85dd43a988a928d0557818d4.png"></img>`,
            "其阳科技",
            "AEWIN",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/5236e6f4e39c49d0ae1b491c735038cf.png"></img>`,
            "兴汉网际",
            `<span class="colorGrass">NEXSEC</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/2e88c33068c04d31a5bb9599c22382a0.png"></img>`,
            "汇志凌云",
            "UNG YUN",
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/a39af7377bbb4860809ab761137bc8ea.png"></img>`,
            "广电五州",
            `<span class="colorGrass">WuZhou</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/b93ab5c255cb4830b2c0b7e09aaced8e.png"></img>`,
            "联软科技",
            `<span class="colorGrass">LEAGSOFT</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/4e59350e44e04e50bff593c080c8a57b.png"></img>`,
            "立华科技",
            `<span class="colorGrass">LS PLAEFORM</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/8d55bacac63a499c9a50c19a996d4cfd.png"></img>`,
            "中科可控",
            `<span class="colorGrass">Suma</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/5739d4caa7214beaa27cc66d10644a62.png"></img>`,
            "安恒信息",
            `<span class="colorGrass">DAS-secunity</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/bce6aa664cd44e76af59ba89e4d4f04d.png"></img>`,
            "网宿科技",
            `<span class="colorGrass">WangSu</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/94df6244d6b04a91b3e8545844bce830.png"></img>`,
            "孝道科技",
            `<span class="colorGrass">DevSecOps</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/ae832a31047749299bd504e6070d487a.png"></img>`,
            "希捷科技",
            `<span class="colorGrass">SEAGATE</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/8dadce3bcf53474b8141421cbc60f360.png"></img>`,
            "安博通",
            `<span class="colorGrass">ABT</span>`,
          ],
          [
            `<img width="60px" style="margin-top:15px;border-radius:50%" src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/4/c39a007819cc484e964e9dbcb8e155c2.png"></img>`,
            "南京壹进制",
            `<span class="colorGrass">cosIc unAry</span>`,
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
