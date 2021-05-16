<template>
  <div class="user-text">
      <div class="page flex-col user-1" v-if="!dy">
      <div class="main1 flex-col">
        <div class="group1 flex-col">
          <img
            class="pic1"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge29bfd29776017f86fcd86aae81629fe2825373b0baae954cfc80134dc78fd8d"
          />
        </div>
      </div>
      <div class="main2 flex-col"></div>
      <div class="main3 flex-col">
        <span class="word1">面对投资盈亏时：</span>
        <span class="txt1">遇到行情波动时：</span>
        <span class="info1">在做投资决策时：</span>
        <span class="info2">遇到投资机会时：</span>
        <span class="txt2">性格分析</span>
        <span class="txt3">不怕犯错，及时止损</span>
        <span class="word2">乐观面对，越跌越买</span>
        <span class="word3">独立决策，犹豫不决</span>
        <span class="word4">不惧风险，博高收益</span>
      </div>
      <div class="main4 flex-col">
        <div class="section1 flex-col">
          <span class="txt4" @click.stop="dy = true">打印我的理财报告</span>
        </div>
        <span class="word5">理财建议</span>
        <span class="txt5">
          在面对市场波动时，保持良好心态，冷静做出决策。保持长期持有的理财习惯，稳中求胜。
        </span>
      </div>
      <div class="main5 flex-col"><span class="word6">后悔</span></div>
      <div class="main6 flex-col"></div>
      <div class="main7 flex-col">
        <div class="outer1 flex-col">
          <div class="bd1 flex-row"><div class="wrap1 flex-col"></div></div>
          <div class="bd2 flex-row"><div class="wrap2 flex-col"></div></div>
          <div class="bd3 flex-row"><div class="main8 flex-col"></div></div>
          <div class="bd4 flex-row"><div class="outer2 flex-col"></div></div>
        </div>
      </div>
      <div class="main9 flex-col"><span class="txt6">乐观</span></div>
      <div class="main10 flex-col"></div>
      <div class="main11 flex-col"><span class="word7">冒险</span></div>
      <div class="main12 flex-col"></div>
      <div class="main13 flex-col"></div>
      <div class="main14 flex-col"><span class="word8">冲动</span></div>
      <div class="main15 flex-col"></div>
      <div class="main16 flex-col"><span class="word9">自信</span></div>
      <div class="main17 flex-col"></div>
      <div class="main18 flex-col"></div>
    </div>
    <div class="page flex-col user-2" v-if="dy">
      <div class="bd1 flex-col">
        <img
          class="pic1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng7a0f37300b3d3ad4bad504f03b45c80a8e9a18de20f32a9e55ddb3fd33d0162f"
        />
        <span class="txt1">理财报告正在打印中，请稍候……</span>
        <img
          class="img1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngf231130124346c5c485d24b6e206571961aec06e0f84cc1540ed3bc417aa28ef"
        />
      </div>
      <div class="bd2 flex-col"></div>
      <div class="bd3 flex-col"></div>
    </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            dy:false
        }
    }
}
</script>

<style lang="scss">
    .user-text{
        html {
  font-size: 18.75px;
}

.page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 102.4rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
  justify-content: flex-start;
  padding-top: 12.827rem;
  align-items: center;
}
.user-1{
    .main1 {
  z-index: 4;
  height: 21.36rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge84aeb8c95d4bac6ff11550f0de6d0bb004b6a1716315f14c8a8d6a95d42b161) -59.5px -59.5px
    no-repeat;
    background-size:100% auto;
  width: 21.12rem;
  justify-content: center;
  align-items: center;
}

.group1 {
  z-index: 8;
  height: 20.134rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2d44a528454dc85bacc8308d8ae8e039477fcf6bae97725d585c8404860a9441)
    100% no-repeat;
    background-size:100% auto;
  width: 20.134rem;
}

.pic1 {
  z-index: 9;
  width: 20.134rem;
  height: 20.134rem;
}

.main2 {
  z-index: 3;
  position: absolute;
  left: -22.826rem;
  top: 34.214rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnga890d1a60155ace076854425fe3b325df2ef2f3f948825cf0eac19d8cd30a4d9)
    418px -9.5px no-repeat;
    background-size:100% auto;
}

.main3 {
  z-index: 5;
  position: absolute;
  left: 2.134rem;
  top: 43.734rem;
  width: 53.334rem;
  height: 30.347rem;
  border-radius: 114px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 50px 10px rgba(0, 0, 0, 0.06);
}

.word1 {
  z-index: 17;
  position: absolute;
  left: 3.227rem;
  top: 23.494rem;
  width: 21.814rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Regular;
  line-height: 3.734rem;
  text-align: left;
}

.txt1 {
  z-index: 16;
  position: absolute;
  left: 3.227rem;
  top: 18.934rem;
  width: 21.814rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Regular;
  line-height: 3.734rem;
  text-align: left;
}

.info1 {
  z-index: 15;
  position: absolute;
  left: 3.227rem;
  top: 14.374rem;
  width: 21.814rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Regular;
  line-height: 3.734rem;
  text-align: left;
}

.info2 {
  z-index: 10;
  position: absolute;
  left: 3.227rem;
  top: 9.814rem;
  width: 21.814rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Regular;
  line-height: 3.734rem;
  text-align: left;
}

.txt2 {
  z-index: 6;
  position: absolute;
  left: 3.227rem;
  top: 2.64rem;
  width: 18.747rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 3.2rem;
  font-family: PingFangSC-Medium;
  line-height: 4.48rem;
  text-align: left;
}

.txt3 {
  z-index: 14;
  position: absolute;
  left: 26.24rem;
  top: 23.494rem;
  width: 24.96rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.word2 {
  z-index: 13;
  position: absolute;
  left: 26.24rem;
  top: 18.934rem;
  width: 24.96rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.word3 {
  z-index: 12;
  position: absolute;
  left: 26.24rem;
  top: 14.374rem;
  width: 24.96rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.word4 {
  z-index: 11;
  position: absolute;
  left: 26.24rem;
  top: 9.814rem;
  width: 24.96rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.main4 {
  z-index: 40;
  height: 22.214rem;
  border-radius: 128px;
  background-color: rgba(23, 88, 255, 1);
  box-shadow: 0px 6px 36px 4px rgba(0, 0, 0, 0.25);
  width: 53.334rem;
  justify-content: flex-end;
  align-items: flex-end;
  position: absolute;
  left: 2.134rem;
  top: 77.014rem;
  padding: 0 80px 76px 0;
}

.section1 {
  z-index: 43;
  position: relative;
  width: 21.014rem;
  height: 4.214rem;
  border-radius: 79px;
  background-color: rgba(255, 255, 255, 1);
}

.txt4 {
  z-index: 44;
  position: absolute;
  left: 2.427rem;
  top: 0.614rem;
  width: 16.16rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.word5 {
  z-index: 41;
  position: absolute;
  left: 3.227rem;
  top: 2.187rem;
  width: 14.934rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 3.2rem;
  font-family: PingFangSC-Medium;
  line-height: 4.48rem;
  text-align: left;
}

.txt5 {
  z-index: 42;
  position: absolute;
  left: 3.227rem;
  top: 9.04rem;
  width: 47.974rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: left;
}

.main5 {
  z-index: 30;
  position: absolute;
  left: 8.774rem;
  top: 14.48rem;
  width: 8.614rem;
  height: 8.614rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng9ece00cdd7b9be452cf31294a0c4dfcda710fc85be2e6ab5e0f98da937f06ee8)
    100% no-repeat;
    background-size:100% auto;
}

.word6 {
  z-index: 39;
  position: absolute;
  left: 1.84rem;
  top: 2.827rem;
  width: 4.934rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  line-height: 2.987rem;
  text-align: center;
}

.main6 {
  z-index: 25;
  position: absolute;
  left: 9.6rem;
  top: 15.36rem;
  width: 6.854rem;
  height: 6.854rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
    100% no-repeat;
    background-size:100% auto;
}

.main7 {
  z-index: 18;
  height: 31.44rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngab1a894c95960b1897c61eb5a1406828906edde8550c5f8e24d17916acf9c303)
    100% no-repeat;
    background-size:100% auto;
  width: 31.44rem;
  justify-content: center;
  align-items: center;
  position: absolute;
  left: 13.067rem;
  top: 7.787rem;
}

.outer1 {
  z-index: 19;
  height: 26.8rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng42fb6a0cc26de5914328930c01ea8354f44aacc4fb0fb9576f01c10d1941dd0f)
    100% no-repeat;
    background-size:100% auto;
  width: 26.8rem;
}

.bd1 {
  z-index: auto;
  width: 0.934rem;
  height: 0.934rem;
  margin: 696px 0 0 30px;
}

.wrap1 {
  z-index: 23;
  width: 0.934rem;
  height: 0.934rem;
  background-color: rgba(23, 88, 255, 0.74);
  border-radius: 50%;
}

.bd2 {
  z-index: auto;
  width: 1.467rem;
  height: 1.467rem;
  margin: -687px 0 0 70px;
}

.wrap2 {
  z-index: 22;
  width: 1.467rem;
  height: 1.467rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.bd3 {
  z-index: auto;
  width: 0.934rem;
  height: 0.934rem;
  margin: 26px 0 0 831px;
}

.main8 {
  z-index: 24;
  width: 0.934rem;
  height: 0.934rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.bd4 {
  z-index: auto;
  width: 1.467rem;
  height: 1.467rem;
  margin: 613px 0 0 880px;
}

.outer2 {
  z-index: 20;
  width: 1.467rem;
  height: 1.467rem;
  background-color: rgba(23, 88, 255, 0.74);
  border-radius: 50%;
}

.main9 {
  z-index: 34;
  position: absolute;
  left: 14.427rem;
  top: 32.187rem;
  width: 8.614rem;
  height: 8.614rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngc508222454860b5eae5acc5d76defbb95e160647914a2c6778d064864dc0c856)
    100% no-repeat;
    background-size:100% auto;
}

.txt6 {
  z-index: 38;
  position: absolute;
  left: 1.84rem;
  top: 2.827rem;
  width: 4.934rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  line-height: 2.987rem;
  text-align: center;
}

.main10 {
  z-index: 29;
  position: absolute;
  left: 15.254rem;
  top: 33.067rem;
  width: 6.854rem;
  height: 6.854rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
    100% no-repeat;
    background-size:100% auto;
}

.main11 {
  z-index: 31;
  position: absolute;
  left: 24.48rem;
  top: 2.667rem;
  width: 8.614rem;
  height: 8.614rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngddffaf4102c62d4d4e107f18282ddef22d75d1b3c225b7450ebd2ce3babaa73b)
    100% no-repeat;
    background-size:100% auto;
}

.word7 {
  z-index: 35;
  position: absolute;
  left: 1.787rem;
  top: 2.827rem;
  width: 4.934rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  line-height: 2.987rem;
  text-align: center;
}

.main12 {
  z-index: 26;
  position: absolute;
  left: 25.307rem;
  top: 3.547rem;
  width: 6.854rem;
  height: 6.854rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
    100% no-repeat;
    background-size:100% auto;
}

.main13 {
  z-index: 21;
  position: absolute;
  left: 28.054rem;
  top: 38.507rem;
  width: 1.467rem;
  height: 1.467rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.main14 {
  z-index: 33;
  position: absolute;
  left: 35.28rem;
  top: 31.68rem;
  width: 8.614rem;
  height: 8.614rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng713cc98b428511a2e7a688bf0ad1528b7c998095d6e526a1b1ad063470b13a11)
    100% no-repeat;
    background-size:100% auto;
}

.word8 {
  z-index: 37;
  position: absolute;
  left: 1.84rem;
  top: 2.827rem;
  width: 4.934rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  line-height: 2.987rem;
  text-align: center;
}

.main15 {
  z-index: 28;
  position: absolute;
  left: 36.107rem;
  top: 32.56rem;
  width: 6.854rem;
  height: 6.854rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
    100% no-repeat;
    background-size:100% auto;
}

.main16 {
  z-index: 32;
  position: absolute;
  left: 40.214rem;
  top: 14.48rem;
  width: 8.614rem;
  height: 8.614rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng5eee85a594afe453f38d6639972d5273f1ade261c44e3eacd1fc4e8af3dd4561)
    100% no-repeat;
    background-size:100% auto;
}

.word9 {
  z-index: 36;
  position: absolute;
  left: 1.787rem;
  top: 2.827rem;
  width: 4.934rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  line-height: 2.987rem;
  text-align: center;
}

.main17 {
  z-index: 27;
  position: absolute;
  left: 41.04rem;
  top: 15.36rem;
  width: 6.854rem;
  height: 6.854rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
    100% no-repeat;
    background-size:100% auto;
}

.main18 {
  z-index: 2;
  position: absolute;
  left: 51.467rem;
  top: 68.027rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2576e4a9e101c98b49f05ddaf263229cec676dafd8b8244a131052f55b22854e) -59.5px -30px
    no-repeat;
    background-size:100% auto;
}
}
.user-2{
    .bd1 {
  z-index: auto;
  width: 57.574rem;
  height: 63.174rem;
}

.pic1 {
  z-index: 6;
  width: 27.707rem;
  height: 19.627rem;
  align-self: flex-end;
  margin-right: 14.854rem;
}

.txt1 {
  z-index: 5;
  width: 57.574rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
  align-self: center;
  margin-top: 4.48rem;
}

.img1 {
  z-index: 4;
  width: 5.52rem;
  height: 3.52rem;
  align-self: flex-end;
  margin: 568.5px 197.5px 0 0;
}

.bd2 {
  z-index: 3;
  position: absolute;
  left: -22.826rem;
  top: 34.214rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnga890d1a60155ace076854425fe3b325df2ef2f3f948825cf0eac19d8cd30a4d9)
    428px -9.5px no-repeat;
    background-size:100% auto;
}

.bd3 {
  z-index: 2;
  position: absolute;
  left: 51.467rem;
  top: 68.027rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2576e4a9e101c98b49f05ddaf263229cec676dafd8b8244a131052f55b22854e) -59.5px -30px
    no-repeat;
    background-size:100% auto;
}
}



    }
</style>