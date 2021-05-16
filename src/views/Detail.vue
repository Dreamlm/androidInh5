<template>
  <div class="detail">
      <div class="page flex-col">
      <div class="mod1 flex-col">
        <img
          @click.stop="toCard"
          class="pic1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng87335a5924bd056f4135617df7b3f97e0acaaa8692fc0cab1f2ee06a5543c07c"
        />
        <img
          class="pic2"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng360160c12efda6e65089b3b4bd0b31965ffdbaabd85f30f6675870e922154572"
        />
        <div class="box1 flex-col"></div>
      </div>
      <div class="mod2 flex-col"></div>
      <img
        class="img1"
        referrerpolicy="no-referrer"
        src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng9285efa49d88f0cb176f40756e1f852cca8e04c2649337d3ad5bdcfa8a51802a"
      />
      <div class="mod3 flex-col">
        <div class="layer1 flex-col">
          <div class="bd1 flex-col">
            <span class="info1">锐意进取策略</span>
            <span class="word1">中高风险</span>
          </div>
          <div class="bd2 flex-col"><div class="bd3 flex-col"></div></div>
          <img
            class="icon1"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng281184381e8f5f270008172635bc913d55ae3371d858b7729763c2f0ded5cd50"
          />
          <div class="bd4 flex-col"></div>
          <div class="bd5 flex-col">
            <span class="txt1">专家会根据行情，结合模型为你调仓</span>
          </div>
          <div class="bd6 flex-col"><span class="word2" @click.stop="toEntry">立即转入</span></div>
          <div class="bd7 flex-col">
            <div class="bd8 flex-col"></div>
            <span class="word3">根据VCMM®模型测算，投资1万并持有3年</span>
            <span class="paragraph1">
              较差情况亏损
              <br />
              不超2340.00元
            </span>
            <span class="paragraph2">
              较好情况可
              <br />
              赚7240.00元
            </span>
          </div>
          <div class="bd9 flex-col">
            <div class="group1 flex-col">
              <div class="outer1 flex-col"></div>
            </div>
            <span class="word4">近一年涨跌幅</span>
            <span class="txt2">+27.70%</span>
            <span class="info2">近一年最大回撤：10.89%</span>
          </div>
          <div class="bd10 flex-col"><div class="layer2 flex-col"></div></div>
          <div class="bd11 flex-col"></div>
        </div>
        <div class="layer3 flex-col"></div>
        <div class="layer4 flex-col"></div>
        <span class="info3">+10%</span>
        <span class="txt3">策略说明</span>
        <span class="txt4">35.00%</span>
        <span class="txt5">股票类基金</span>
        <span class="word5">65.00%</span>
        <span class="txt6">固收类基金</span>
        <span class="word6">投后有顾</span>
        <span class="word7">优选基金</span>
        <span class="info4">定制策略</span>
      </div>
      <div class="mod4 flex-col"></div>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{

        }
    },
    methods:{
        toEntry(){
            this.$router.push({path:'/entry'})
        },
        toCard(){
            this.$router.push({path:'/card'})
        }
    }
}
</script>

<style lang="scss">
html {
  font-size: 18.75px;
}
.detail{

    html {
  font-size: 37.5px;
}

.page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 163.654rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
  justify-content: flex-end;
  padding-bottom: 0;
}

.mod1 {
  z-index: auto;
  width: 57.6rem;
  height: 161.334rem;
}

.pic1 {
  z-index: 34;
  width: 3.76rem;
  height: 3.094rem;
  align-self: flex-end;
  margin-right: 2.427rem;
}

.pic2 {
  z-index: 53;
  width: 3.174rem;
  height: 1.974rem;
  align-self: center;
  margin-top: 0.88rem;
}

.box1 {
  z-index: 2;
  width: 57.6rem;
  height: 70rem;
  background-color: rgba(23, 88, 255, 1);
  align-self: center;
  margin-top: 85.387rem;
}

.mod2 {
  z-index: 4;
  position: absolute;
  left: -22.213rem;
  top: 6.454rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
    416.5px -16px no-repeat;
    background-size:100% auto;
}

.img1 {
  z-index: 6;
  position: absolute;
  left: 0;
  top: 53.174rem;
  width: 57.6rem;
  height: 56.56rem;
}

.mod3 {
  z-index: 7;
  height: 149.734rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 50px 10px rgba(0, 0, 0, 0.06);
  width: 48.214rem;
  justify-content: flex-start;
  position: absolute;
  left: 4.72rem;
  top: 9.28rem;
}

.layer1 {
  z-index: auto;
  width: 48.214rem;
  height: 143.92rem;
}

.bd1 {
  z-index: 8;
  position: relative;
  width: 48.214rem;
  height: 8.134rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng8270262c6db1ff2eb8d495807fd3d50e960e2b69e1b676e1bb4738a00ba607db) -54px -58.5px
    no-repeat;
    background-size:112% auto;
  align-self: center;
}

.info1 {
  z-index: 33;
  position: absolute;
  left: 13.627rem;
  top: 0.96rem;
  width: 20.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(191, 80, 29, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Semibold;
  line-height: 3.734rem;
  text-align: center;
}

.word1 {
  z-index: 16;
  position: absolute;
  left: 20.614rem;
  top: 4.96rem;
  width: 6.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(191, 80, 29, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.bd2 {
  z-index: 17;
  height: 18.507rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngf6ad1e920bffb8cd513c4b34a1e126eb1979b4304a7db141d523fa74b70c1b26) -0.5px
    0px no-repeat;
    background-size:100% auto;
  align-self: center;
  margin-top: 10.774rem;
  width: 26rem;
  justify-content: center;
  align-items: center;
}

.bd3 {
  z-index: 40;
  width: 9.254rem;
  height: 2.854rem;
  border-radius: 26.75px 26.75px 26.75px 26.75px;
  border: 2px solid rgba(151, 151, 151, 1);
}

.icon1 {
  z-index: 41;
  width: 1.014rem;
  height: 0.987rem;
  align-self: flex-start;
  margin: 67px 0 0 273px;
}

.bd4 {
  z-index: 42;
  width: 1.014rem;
  height: 1.014rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
  align-self: flex-start;
  margin: 28px 0 0 273px;
}

.bd5 {
  z-index: 43;
  position: relative;
  width: 29.04rem;
  height: 3.68rem;
  border-radius: 69px;
  background-color: rgba(23, 88, 255, 0.21);
  align-self: flex-end;
  margin: 42px 179px 0 0;
}

.txt1 {
  z-index: 47;
  position: absolute;
  left: 1.44rem;
  top: 0.774rem;
  width: 26.027rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.bd6 {
  z-index: 44;
  position: relative;
  width: 45.2rem;
  height: 6.267rem;
  border-radius: 8.5px;
  background-color: rgba(23, 88, 255, 1);
  align-self: flex-start;
  margin: 28.5px 0 0 27.5px;
}

.word2 {
  z-index: 48;
  position: absolute;
  left: 12.214rem;
  top: 1.147rem;
  width: 20.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
}

.bd7 {
  z-index: 45;
  height: 8.534rem;
  border-radius: 17px;
  background-color: rgba(236, 236, 236, 1);
  align-self: flex-start;
  width: 45.2rem;
  justify-content: flex-end;
  padding-bottom: 0.88rem;
  align-items: center;
  position: relative;
  margin: 27.5px 0 0 27.5px;
}

.bd8 {
  z-index: 52;
  width: 0.027rem;
  height: 3.36rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngc43c18cbfa6ae0ed6f8026c0caad0a90920691edcdaa731305298ee8ad5c043e)
    100% no-repeat;
    background-size:100% auto;
}

.word3 {
  z-index: 49;
  position: absolute;
  left: 9.52rem;
  top: 0.72rem;
  width: 26.16rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(147, 147, 147, 1);
  font-size: 1.333rem;
  font-family: PingFangSC-Regular;
  line-height: 1.867rem;
  text-align: center;
}

.paragraph1 {
  z-index: 51;
  position: absolute;
  left: 25.094rem;
  top: 3.467rem;
  width: 9.494rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(147, 147, 147, 1);
  font-size: 1.333rem;
  font-family: PingFangSC-Regular;
  line-height: 1.867rem;
  text-align: left;
}

.paragraph2 {
  z-index: 50;
  position: absolute;
  left: 12.08rem;
  top: 3.467rem;
  width: 8.027rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(147, 147, 147, 1);
  font-size: 1.333rem;
  font-family: PingFangSC-Regular;
  line-height: 1.867rem;
  text-align: right;
}

.bd9 {
  z-index: 46;
  height: 14.507rem;
  background-color: rgba(23, 88, 255, 0.09);
  align-self: flex-start;
  width: 45.2rem;
  justify-content: flex-start;
  padding-top: 2.534rem;
  align-items: flex-end;
  position: relative;
  margin: 55px 0 0 55px;
}

.group1 {
  z-index: 60;
  height: 5.254rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng9bb8ddae5effe775e2751e0a8b72178ab4247363b0dd9b6b9e31bf65de149fee)
    1px 0px no-repeat;
    background-size:100% auto;
  width: 27.174rem;
}

.outer1 {
  z-index: 61;
  width: 27.174rem;
  height: 5.254rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng7bcf312072cd011f2a572705dba82f282c46c53fe5962a4e364d1a9ca77e735b) -3px -4px
    no-repeat;
    background-size:100% auto;
}

.word4 {
  z-index: 54;
  position: absolute;
  left: 2.027rem;
  top: 1.947rem;
  width: 11.6rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: left;
}

.txt2 {
  z-index: 55;
  position: absolute;
  left: 2rem;
  top: 5.787rem;
  width: 16.374rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(230, 16, 16, 1);
  font-size: 2.4rem;
  font-family: PingFangSC-Semibold;
  line-height: 3.36rem;
  text-align: left;
}

.info2 {
  z-index: 59;
  position: absolute;
  left: 2rem;
  top: 10.614rem;
  width: 18.667rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: left;
}

.bd10 {
  z-index: 62;
  height: 0.054rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdb136d154d18242073845c04d5c844c91df6355233719ea187f3f14d9923274d) -1px
    0px no-repeat;
    background-size:100% auto;
  align-self: flex-start;
  width: 44.934rem;
  align-items: flex-start;
  padding-left: 1.174rem;
  margin: 142px 0 0 27.5px;
}

.layer2 {
  z-index: 63;
  width: 10.214rem;
  height: 0.054rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng40e30151a2135291c05fb4871b0e786bcf0a585a5ceb92cd1caf06760786824b) -4px -3px
    no-repeat;
    background-size:100% auto;
}

.bd11 {
  z-index: 64;
  width: 46.507rem;
  height: 49.787rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng68b0a36073de9a61271041a60d0b5c98689f48ade6c1ddabc53fdb1eb7580125) -1px
    0px no-repeat;
    background-size:100% auto;
  align-self: center;
  margin-top: 2.347rem;
}

.layer3 {
  z-index: 22;
  position: absolute;
  left: 24.107rem;
  top: 11.36rem;
  width: 13.04rem;
  height: 14.347rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngeaf48cacc5b17289dadc3b37fa6e2d8f662ab6ac6dd2138268b1d4bd208968af) -1px
    0px no-repeat;
    background-size:100% auto;
}

.layer4 {
  z-index: 27;
  position: absolute;
  left: 12.187rem;
  top: 11.36rem;
  width: 11.947rem;
  height: 9.68rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng43f623c2048978af1ed888f88144ef176be55dbc6211bc34dc8ce967f3eb2d0a) -1px
    0px no-repeat;
    background-size:100% auto;
}

.info3 {
  z-index: 32;
  position: absolute;
  left: 17.6rem;
  top: 19.894rem;
  width: 13.04rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 3.733rem;
  font-family: PingFangSC-Semibold;
  line-height: 5.227rem;
  text-align: center;
}

.txt3 {
  z-index: 11;
  position: absolute;
  left: 20.667rem;
  top: 27.04rem;
  width: 6.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(143, 143, 143, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.txt4 {
  z-index: 14;
  position: absolute;
  left: 26.56rem;
  top: 40.267rem;
  width: 7.067rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(230, 16, 16, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Medium;
  line-height: 2.24rem;
  text-align: center;
}

.txt5 {
  z-index: 12;
  position: absolute;
  left: 17.174rem;
  top: 40.267rem;
  width: 8.72rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.word5 {
  z-index: 15;
  position: absolute;
  left: 26.56rem;
  top: 42.72rem;
  width: 7.067rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Medium;
  line-height: 2.24rem;
  text-align: center;
}

.txt6 {
  z-index: 13;
  position: absolute;
  left: 17.174rem;
  top: 42.774rem;
  width: 8.72rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.word6 {
  z-index: 58;
  position: absolute;
  left: 35.334rem;
  top: 87.787rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 2.4rem;
  font-family: PingFangSC-Medium;
  line-height: 3.36rem;
  text-align: center;
}

.word7 {
  z-index: 57;
  position: absolute;
  left: 19.494rem;
  top: 87.787rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 2.4rem;
  font-family: PingFangSC-Medium;
  line-height: 3.36rem;
  text-align: center;
}

.info4 {
  z-index: 56;
  position: absolute;
  left: 2.64rem;
  top: 87.787rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.4rem;
  font-family: PingFangSC-Medium;
  line-height: 3.36rem;
  text-align: center;
}

.mod4 {
  z-index: 3;
  position: absolute;
  left: 51.094rem;
  top: 69.76rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge754fb8dd9256facbb96fdd691507f3a654d6c45789681baa139b08626c0b012) -119px -65px
    no-repeat;
    background-size:100% auto;
}




}
</style>