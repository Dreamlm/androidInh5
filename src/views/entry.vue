<template>
  <div class="entry" v-if="!end">
      <div class="page flex-col">
      <div class="wrap1 flex-row">
        <img
            @click.stop="backA"
          class="img1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbaee696ebb27ebb019468d44c8ac7bcabe494e65c8fab569c6560fcd63f4aec0"
        />
        <img
            @click.stop="toCard"
          class="pic1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng87335a5924bd056f4135617df7b3f97e0acaaa8692fc0cab1f2ee06a5543c07c"
        />
      </div>
      <div class="wrap2 flex-col"></div>
      <div class="wrap3 flex-col">
        <div class="outer1 flex-col">
          <div class="layer1 flex-row">
            <div class="bd1 flex-col"><span class="word1">5000元</span></div>
            <div class="bd2 flex-col"><span class="txt1">6000元</span></div>
            <div class="bd3 flex-col"><span class="txt2">8000元</span></div>
          </div>
          <div class="layer2 flex-col"></div>
          <div class="layer3 flex-col"></div>
          <div class="layer4 flex-col"></div>
          <div class="layer5 flex-col">
            <img
              class="img2"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng9c59d64b8880ef5a1dc3376ffc00b2856b1f4e6f2bf1cb39316af3af0e9cc1a9"
            />
            <span class="word2" @click.stop="end = true">扫码立即转入</span>
          </div>
          <div class="layer6 flex-col"></div>
        </div>
        <span class="txt3">转入金额</span>
        <span class="txt4">交易规则</span>
        <span class="info1">￥</span>
        <span class="txt5">
            <input type="text" placeholder="100.00元起购" v-model="num"/>
        </span>
        <span class="paragraph1">
          确认时间：现在转入，预计04月14日（星期三）24点前确认份额。
          <br />
          转入费率：基金交易相关费用按照基金产品收费规则收取。
        </span>
        <span class="word3">
          请在下方展示付款码进行交易，您将获取一张实体理财卡，请注意保存，市场有风险，投资需谨慎。
        </span>
      </div>
      <div class="wrap4 flex-col">
        <span class="word4">锐意进取策略</span>
        <span class="word5">中高风险</span>
      </div>
      <div class="wrap5 flex-col"></div>
    </div>
  </div>
  <div class="end" v-if="end">
      <div class="page flex-col">
      <div class="box1 flex-col"></div>
      <div class="box2 flex-col">
        <div class="box3 flex-col">
          <div class="box4 flex-col">
            <div class="layer1 flex-col">
              <img
                class="img1"
                referrerpolicy="no-referrer"
                src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng7be82cf0f6e69ce750b1229c2753f3108dfbea31c36ce731a31f56583100c8af"
              />
              <img
                class="pic1"
                referrerpolicy="no-referrer"
                src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngb87b45c6ff4bb79d07720effeaa5a9ae311d91bba6861727806ead89a363d214"
              />
              <img
                class="img2"
                referrerpolicy="no-referrer"
                src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngee57abf5b01afb893071976687d2e41cccbd1305f9fa2efd97b0179a1da0da72"
              />
            </div>
            <div class="layer2">
              <span class="word1">Li，</span>
              <span class="word2">购买成功！</span>
            </div>
            <div class="layer3 flex-col"></div>
            <span class="word3">请在下方领取您的专属理财卡！</span>
          </div>
          <div class="box5 flex-col" @click.stop="toCard"><span class="txt1">完成</span></div>
        </div>
      </div>
      <div class="box6 flex-col">
        <div class="box7 flex-col"></div>
        <span class="info1">转入金额</span>
        <span class="info2">交易规则</span>
        <span class="word4">￥</span>
        <span class="word5">100.00元起购</span>
        <span class="word6">8000元</span>
        <span class="txt2">6000元</span>
        <span class="word7">5000元</span>
        <span class="paragraph1">
          确认时间：现在转入，预计04月14日（星期三）24点前确认份额。
          <br />
          转入费率：基金交易相关费用按照基金产品收费规则收取。
        </span>
        <span class="txt3">扫码立即转入</span>
        <span class="info3">
          请在下方展示付款码进行交易，您将获取一张实体理财卡，请注意保存，市场有风险，投资需谨慎。
        </span>
      </div>
      <div class="box8 flex-col">
        <span class="word8">锐意进取策略</span>
        <span class="word9">中高风险</span>
      </div>
      <div class="box9 flex-col"></div>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            num:'',
            end:false
        }
    },
    methods:{
        backA(){
            this.$router.go(-1);
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



    .entry{
        .page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 102.4rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
  justify-content: flex-start;
  padding-top: 2.32rem;
  align-items: center;
}

.wrap1 {
  z-index: auto;
  width: 52.72rem;
  height: 3.094rem;
  justify-content: space-between;
}

.img1 {
  z-index: 3;
  width: 1.707rem;
  height: 3.094rem;
}

.pic1 {
  z-index: 5;
  width: 3.76rem;
  height: 3.094rem;
}

.wrap2 {
  z-index: 2;
  position: absolute;
  left: -22.213rem;
  top: 6.454rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
    416.5px -16px no-repeat;
    background-size:100% auto;
}

.wrap3 {
  z-index: 12;
  height: 87.814rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 50px 10px rgba(0, 0, 0, 0.06);
  width: 48.214rem;
  justify-content: flex-end;
  align-items: flex-end;
  position: absolute;
  left: 4.694rem;
  top: 9.254rem;
  padding: 0 24.5px 53.5px 0;
}

.outer1 {
  z-index: auto;
  width: 45.2rem;
  height: 58.294rem;
}

.layer1 {
  z-index: auto;
  width: 44.347rem;
  height: 3.68rem;
  margin-left: 0.32rem;
  justify-content: space-between;
}

.bd1 {
  z-index: 24;
  position: relative;
  width: 13.574rem;
  height: 3.68rem;
  border-radius: 34.5px;
  background-color: rgba(23, 88, 255, 0.21);
}

.word1 {
  z-index: 27;
  position: absolute;
  left: 1.734rem;
  top: 0.534rem;
  width: 10.134rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.bd2 {
  z-index: 25;
  position: relative;
  width: 13.574rem;
  height: 3.68rem;
  border-radius: 69px;
  background-color: rgba(23, 88, 255, 0.21);
}

.txt1 {
  z-index: 29;
  position: absolute;
  left: 1.734rem;
  top: 0.534rem;
  width: 10.134rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.bd3 {
  z-index: 26;
  position: relative;
  width: 13.574rem;
  height: 3.68rem;
  border-radius: 34.5px;
  background-color: rgba(23, 88, 255, 0.21);
}

.txt2 {
  z-index: 30;
  position: absolute;
  left: 1.734rem;
  top: 0.534rem;
  width: 10.134rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.layer2 {
  z-index: 14;
  width: 44.934rem;
  height: 0.054rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdb136d154d18242073845c04d5c844c91df6355233719ea187f3f14d9923274d) -0.5px
    0px no-repeat;
    background-size:100% auto;
  align-self: flex-start;
  margin-top: 2.667rem;
}

.layer3 {
  z-index: 31;
  width: 0.8rem;
  height: 0.8rem;
  background-color: rgba(172, 172, 172, 1);
  border-radius: 50%;
  align-self: flex-start;
  margin: 71.5px 0 0 6.5px;
}

.layer4 {
  z-index: 32;
  width: 0.8rem;
  height: 0.8rem;
  background-color: rgba(172, 172, 172, 1);
  border-radius: 50%;
  align-self: flex-start;
  margin: 83px 0 0 6.5px;
}

.layer5 {
  z-index: 33;
  height: 6.267rem;
  border-radius: 17px;
  background-color: rgba(23, 88, 255, 1);
  align-self: center;
  margin-top: 9.227rem;
  width: 45.2rem;
  justify-content: center;
  align-items: flex-start;
  padding-left: 11.547rem;
  position: relative;
}

.img2 {
  z-index: 35;
  width: 2.454rem;
  height: 2.347rem;
}

.word2 {
  z-index: 34;
  position: absolute;
  left: 12.774rem;
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

.layer6 {
  z-index: 42;
  width: 19.947rem;
  height: 13.974rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng8270a479f80bf68f4ae19222a140acf9ad810ed3b05b33dd8e773f54818f416c)
    100% no-repeat;
    background-size:100% auto;
  align-self: flex-start;
  margin: 236px 0 0 233px;
}

.txt3 {
  z-index: 20;
  position: absolute;
  left: 2.027rem;
  top: 11.814rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 2.4rem;
  font-family: PingFangSC-Medium;
  line-height: 3.36rem;
  text-align: center;
}

.txt4 {
  z-index: 22;
  position: absolute;
  left: 38.347rem;
  top: 12.027rem;
  width: 7.6rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: right;
}

.info1 {
  z-index: 21;
  position: absolute;
  left: 2.027rem;
  top: 17.414rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 5.333rem;
  font-family: PingFangSC-Medium;
  line-height: 7.467rem;
  text-align: left;
}

.txt5 {
  z-index: 23;
  position: absolute;
  left: 7.12rem;
  top: 20.027rem;
  width: 13.574rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(172, 172, 172, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
  input{
      width:100%;
      height:3rem;
      border:none;
      font-size:2rem;
  }
}

.paragraph1 {
  z-index: 28;
  position: absolute;
  left: 3.787rem;
  top: 35.92rem;
  width: 42.614rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(172, 172, 172, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Regular;
  line-height: 2.614rem;
  text-align: left;
}

.word3 {
  z-index: 13;
  position: absolute;
  left: 2.8rem;
  top: 62.134rem;
  width: 42.614rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.wrap4 {
  z-index: 15;
  position: absolute;
  left: 4.774rem;
  top: 9.28rem;
  width: 48.214rem;
  height: 8.134rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng8270262c6db1ff2eb8d495807fd3d50e960e2b69e1b676e1bb4738a00ba607db) -59px -59.5px
    no-repeat;
    background-size:113% auto;
}

.word4 {
  z-index: 19;
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

.word5 {
  z-index: 18;
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

.wrap5 {
  z-index: 11;
  position: absolute;
  left: 51.414rem;
  top: 69.307rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6e7aff12b40a4794584456e61a45b32447c004658913bbafa7ba097d46d7abda) -59.5px -30px
    no-repeat;
}
    }
    .end{
        .page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 102.4rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
}

.box1 {
  z-index: 2;
  position: absolute;
  left: -22.213rem;
  top: 6.454rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
    833px -32px no-repeat;
}

.box2 {
  z-index: 38;
  height: 102.4rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6448999ae7ccf0fcc2b6b14ac883fb7edfcffeaff3c967aab05fd28aea8afc97)
    100% no-repeat;
  width: 57.6rem;
  justify-content: flex-start;
  padding-top: 12.24rem;
  align-items: center;
  position: absolute;
  left: 0;
  top: 0;
}

.box3 {
  z-index: auto;
  width: 48.214rem;
  height: 73.2rem;
}

.box4 {
  z-index: 39;
  height: 62.267rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 100px 20px rgba(0, 0, 0, 0.06);
  align-self: center;
  width: 48.214rem;
  justify-content: flex-end;
  padding-bottom: 1.2rem;
  align-items: center;
  position: relative;
}

.layer1 {
  z-index: auto;
  width: 25.734rem;
  height: 46.587rem;
}

.img1 {
  z-index: 93;
  width: 10.107rem;
  height: 10.107rem;
  align-self: center;
}

.pic1 {
  z-index: 40;
  width: 25.734rem;
  height: 22.08rem;
  align-self: center;
  margin-top: 3.867rem;
}

.img2 {
  z-index: 102;
  width: 3.174rem;
  height: 1.974rem;
  align-self: center;
  margin-top: 8.56rem;
}

.layer2 {
  z-index: 92;
  position: absolute;
  left: 7.094rem;
  top: 4.694rem;
  width: 34.027rem;
  height: 6.72rem;
  overflow-wrap: break-word;
  text-align: center;
  font-size: 0;
}

.word1 {
  font-size: 3.733rem;
  font-family: PingFangSC-Medium;
  color: rgba(0, 0, 0, 1);
  line-height: 5.227rem;
}

.word2 {
  font-size: 3.733rem;
  font-family: PingFangSC-Medium;
  color: rgba(23, 88, 255, 1);
  line-height: 5.227rem;
}

.layer3 {
  z-index: 98;
  position: absolute;
  left: 17.867rem;
  top: 13.28rem;
  width: 12.507rem;
  height: 12.507rem;
  border: 1px solid rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.word3 {
  z-index: 101;
  position: absolute;
  left: 4.107rem;
  top: 53.707rem;
  width: 42.614rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.box5 {
  z-index: 99;
  position: relative;
  width: 18.587rem;
  height: 6.694rem;
  border-radius: 125.5px 125.5px 125.5px 125.5px;
  background-color: rgba(23, 88, 255, 1);
  align-self: center;
  margin-top: 4.24rem;
}

.txt1 {
  z-index: 100;
  position: absolute;
  left: 4.214rem;
  top: 1.494rem;
  width: 10.16rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
}

.box6 {
  z-index: 4;
  height: 87.814rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 100px 20px rgba(0, 0, 0, 0.06);
  width: 48.214rem;
  justify-content: flex-end;
  padding-bottom: 2.854rem;
  align-items: center;
  position: absolute;
  left: 4.694rem;
  top: 9.254rem;
}

.box7 {
  z-index: 27;
  width: 19.947rem;
  height: 13.974rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng8270a479f80bf68f4ae19222a140acf9ad810ed3b05b33dd8e773f54818f416c)
    100% no-repeat;
}

.info1 {
  z-index: 12;
  position: absolute;
  left: 2.027rem;
  top: 11.814rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 2.4rem;
  font-family: PingFangSC-Medium;
  line-height: 3.36rem;
  text-align: center;
}

.info2 {
  z-index: 14;
  position: absolute;
  left: 38.347rem;
  top: 12.027rem;
  width: 7.6rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: right;
}

.word4 {
  z-index: 13;
  position: absolute;
  left: 2.027rem;
  top: 17.414rem;
  width: 10.187rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 5.333rem;
  font-family: PingFangSC-Medium;
  line-height: 7.467rem;
  text-align: left;
}

.word5 {
  z-index: 15;
  position: absolute;
  left: 7.12rem;
  top: 20.027rem;
  width: 13.574rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(172, 172, 172, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.word6 {
  z-index: 22;
  position: absolute;
  left: 34.534rem;
  top: 27.2rem;
  width: 10.134rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.txt2 {
  z-index: 21;
  position: absolute;
  left: 19.147rem;
  top: 27.2rem;
  width: 10.134rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.word7 {
  z-index: 19;
  position: absolute;
  left: 3.76rem;
  top: 27.2rem;
  width: 10.134rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.paragraph1 {
  z-index: 20;
  position: absolute;
  left: 3.787rem;
  top: 35.92rem;
  width: 42.614rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(172, 172, 172, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Regular;
  line-height: 2.614rem;
  text-align: left;
}

.txt3 {
  z-index: 26;
  position: absolute;
  left: 13.92rem;
  top: 53.28rem;
  width: 20.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
}

.info3 {
  z-index: 5;
  position: absolute;
  left: 2.8rem;
  top: 62.134rem;
  width: 42.614rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.box8 {
  z-index: 7;
  position: absolute;
  left: 4.774rem;
  top: 9.28rem;
  width: 48.214rem;
  height: 8.134rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng8270262c6db1ff2eb8d495807fd3d50e960e2b69e1b676e1bb4738a00ba607db) -118px -119px
    no-repeat;
}

.word8 {
  z-index: 11;
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

.word9 {
  z-index: 10;
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

.box9 {
  z-index: 3;
  position: absolute;
  left: 51.414rem;
  top: 69.307rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6e7aff12b40a4794584456e61a45b32447c004658913bbafa7ba097d46d7abda) -119px -60px
    no-repeat;
}

    }
</style>