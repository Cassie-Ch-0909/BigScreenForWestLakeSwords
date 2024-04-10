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
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月8日&nbsp;&nbsp;&nbsp;&nbsp;13:00-18:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MSS安全托管运营服务论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">做网络安全，既要低头拉车，也要抬头看路</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/45d698748a394f6e923254d06ffdcc76.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>左晓栋</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国科学技术大学网络空间安全学院教授、科技人文高等研究院副院长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月2日&nbsp;&nbsp;&nbsp;&nbsp;08:45 -12:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;开幕式及全体大会</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">探索未来数字世界 让安全成为发展的一部分</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/416955f5d3a34eda8b95411dd0483065.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>崔光耀</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>《中国信息安全》杂志原主编</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月2日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;杭州论坛：数字化改革主题论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">“一以贯之”其一，要持之以恒地加强网络安全的顶层设计。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/2f791d88ef5c42669d61dfb560ab484e.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>李新友</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>国家安全信息安全员</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月2日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;北京论坛：网络安全趋势论坛（闭门）</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">网络安全工作的两项重点，分别是关键信息基础设施保护和数据安全。‍‍</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/54400aca0eea438f822ebf3a059e43db.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>曲胜</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国能源研究会能源网络安全技术研究中心常务副主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;14:00-17:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;当科幻照进现实我们会更安全吗？</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">两个“新”，其一是‍‍新的产业方向,其二是新的威胁对策。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/82f148791fda423aac58841930ca293c.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>王秉政</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>全国信安委成员</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;09:00-12:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;威胁情报及应急响应论坛（闭门）</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">数字城市的建设成果 安全必将是重要一环</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/e93465d2e3bf4d3d8f9cce134f7cceec.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>许玉娜</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国网络安全产业联盟副秘书长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;08:40-12:25&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;安全托管运营服务论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">厘清重要数据 是保障数据安全的基础</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/d3fc25a6b3c84ebc98e154893a49ac40.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>严明</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国计算机学会计算机安全专委会荣誉主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;08:40-12:02&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;关键信息基础设施及等级保护论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">企业信息安全建设的难点在于人的治理。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/4075600edb5c4360a406fa920ea32c86.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>姚力</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>CNCERT 博士</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;工业领域网络和数据安全论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">数字化转型会是未来主流的方向。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/517e9a9d04484be38c37f406dd3fb9c1.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>叶红</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国信息协会信息安全专业委员会主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数据安全治理和个人信息保护论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">成本优化应该是未来的一个主流趋势。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="	https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/043e77f57ca444eea78c05f3e2ef7747.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>张莹</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>国家工业信息安全发展研究中心网络安全宣传部主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;14:00-15:20&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网络安全科普论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">未来所有的安全风险的管控和治理，都将以数据安全为核心。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/9be725f9fc34436d8d0a701923f4a2e5.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>沈韵</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江省互联网协会副理事长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;信创与密码应用论坛（下）</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">做安全不是看谁做的好，而是看谁做的最烂。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/63c23cf679a449ffb53a17bdef1115de.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>傅正</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江省图灵互联网研究院院长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月5日&nbsp;&nbsp;&nbsp;&nbsp;18:00-21:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;格致论道@西湖论剑</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">没有安全事件，不等于你很安全。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/beb377784b8a453b9a071a8565990e7e.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>黄益超</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江省智慧城市促进会常务副秘书长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月5日&nbsp;&nbsp;&nbsp;&nbsp;10:00-10:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;95后极客青年Talk</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">针对勒索病毒也是需要大家在各个维度去提升自己，增强自己对于安全的感知能力。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/c778d8425ec84a28aedef86301358333.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>施雄伟</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>杭州亚组委信息技术部副部长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月6日&nbsp;&nbsp;&nbsp;&nbsp;13:00-13:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;当科幻照进现实我们会更安全吗？</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">没有绝对的安全。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/c9a9c9abb84a4a9da5cc4fb774cefa35.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>许绍州</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江省委机要局原局长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月6日&nbsp;&nbsp;&nbsp;&nbsp;15:00-15:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;人工智能会颠覆安全行业吗？</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">中国的企业在信息化发展的速度是很快的，但是防护的能力是极弱的。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/564e0c3b11904cc9a45af0b45c9c292c.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>尹本臻</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江省数字经济联合会秘书长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;08:40-12:25&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;关键信息基础设施及等级保护论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">核心数据保护好。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/8c890dc751a949bdbe88165429b3032e.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>郁全胜</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙大城市学院城市大脑研究院副院长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月3日&nbsp;&nbsp;&nbsp;&nbsp;08:40-12:02&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;信创与密码应用论坛（上）</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">大规模的增强企业的防护和检测能力。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/0d712721dba548e193e308a1f9fbbe3d.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>冯燕春</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国电子商会自主创新与安全技术委员会理事长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月6日&nbsp;&nbsp;&nbsp;&nbsp;15:30-16:40&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;反诈直播间@西湖论剑</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">检测能力的增强是现在企业非常需要去快速增大投入的部分。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/73792f156e244136b258685ce2c26611.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>杨建军</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>全国信安标委秘书长、中国电子技术标准化研究院党委书记、副院长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;13:30-18:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数字中国&安全治理论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">应用相关的标准来对企业这方面的安全能力进行评估。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/0c3872364b7049039d56d813198a336a.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>魏亮</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国信息通信研究院副院长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:10&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;当科幻照进现实我们会更安全吗？</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">增强应对勒索软件攻击的防护能力是需要从多个维度去全面考量。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/2713698b09004115840e6867ab347579.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>马晓军</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江省委网信办副主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;车联网安全论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">数字经济更需要成为“可信经济”。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/29445b328ce7488199c2c128bac6ff44.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>严寒冰</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>国家互联网应急中心运行部主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;09:00-12:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;主论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">实现数据的不外泄。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/5e081c17adc34a27bd7bba87c6ec59d4.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>俞克群</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>国家信息技术安全研究中心主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;工业领域网络和数据安全论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">政务数据共享是其中的支撑和枢纽。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/ddd21a10f120464b94cb2749398ef9f6.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>齐同军</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>杭州市数据资源管理局党组成员、数据资源处处长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:50&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;网络安全创新发展高端论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">政务数据呈现出层级分布的特点。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/866c2800369f4b2790ee04b05169becb.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>顾嘉福</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>原中央网信办国家计算机网络与信息安全管理中心上海分中心党委书记、主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;13:30-17:30&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;企业数据安全治理论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">建立数据安全共享体系。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/f719343836904be2b1490d423623025f.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>倪荣</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江大学公共卫生学院研究员</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;12:00-14:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;独家探营.数字安全创新成果发展</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">数字治理的核心要素是大数据。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/e66888065fcb4b23a90d193ea6746e2e.jpg"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>李冰</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>原国家信息技术安全研究中心副主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月7日&nbsp;&nbsp;&nbsp;&nbsp;09:00-22:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;生态合作伙伴分论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">筑牢‘制度、技术、管理’三道防火墙，夯实安全底座。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/22a1b6c5e9c049a6be23d2b11f3244a1.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>赵宏志</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>中国网络空间安全协会副秘书长</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月8日&nbsp;&nbsp;&nbsp;&nbsp;08:30-12:10&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;教育技术产业融合创新发展论坛</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">纵向监督、横向联动。</p>
      </div>  
  </div>`,
          ],
          [
            `<div style="width:600px;height:410px;">
      <div style="width:600px;height:150px; display:flex; align-items: center;justify-content: space-between; padding-left:10px;padding-right:10px">
        <img style='width: 120px;height: 120px;border-radius: 50%;' src="https://obs-xhlj.obs.cn-east-3.myhuaweicloud.com/2023/3/22a1b6c5e9c049a6be23d2b11f3244a1.png"></img>  
        <div style=" width: 420px; height: 130px; color:black;">
        <p style="margin-top: -130px; font-size:30px" class='colorGrass'>陈文智</p>  
        <p style="margin-top: -290px; font-size:20px" class='colorGrass'>浙江大学公信息中心主任</p>  
        </div>
      </div>
      <div style="width:600px;height:150px;position:relative;">
        <p style="color:white;position:absolute;left:20px;top:-145px;font-size:20px " class="colorBlue">议程信息：</p>
        <p style="color:white;position:absolute;left:20px;top:-105px;font-size:20px">5月8日&nbsp;&nbsp;&nbsp;&nbsp;09:00-12:00&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;商用密码应用</p>
        <p style="color:white;position:absolute;left:20px;top:-65px;font-size:20px" class="colorBlue">访谈语录：</p>
        <p style="color:white;position:absolute;left:20px;top:-25px;font-size:20px">提升管理效率和应急响应能力。</p>
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
