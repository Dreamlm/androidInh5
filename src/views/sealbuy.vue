<template>
  <div class="sealbuy">
      <div class="page flex-col">
      <img
        @click.stop="backTo"
        class="pic1"
        referrerpolicy="no-referrer"
        src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbaee696ebb27ebb019468d44c8ac7bcabe494e65c8fab569c6560fcd63f4aec0"
      />
      <div class="layer1 flex-col"></div>
      <div class="layer2 flex-col">
        <div class="wrap1 flex-col">
          <div class="block1 flex-col">
            <div class="group1 flex-col">
              <span class="info1">8462&nbsp;8383&nbsp;1988&nbsp;4282</span>
            </div>
            <img
              class="pic2"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng96ca4c1788fa33bc4bb45b8100ee0927220cae9fe2806400e0f79ca8cc18c73c"
            />
          </div>
          <div class="block2 flex-col"></div>
          <img
            class="img1"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngee57abf5b01afb893071976687d2e41cccbd1305f9fa2efd97b0179a1da0da72"
          />
          <div class="block3 flex-col"><span class="word1" @click.stop="sealTo">确认卖出</span></div>
        </div>
        <span class="txt1">总金额</span>
        <span class="word2">1107.47</span>
        <span class="info2">累计收益（元）</span>
        <span class="txt2">持有收益（元）</span>
        <span class="word3">昨日收益（元）</span>
        <span class="word4">107.47</span>
        <span class="info3">107.47</span>
        <span class="word5">+2.14</span>
        <span class="word6">请将您的理财卡插入下方卡槽进行交易！</span>
      </div>
      <div class="layer3 flex-col"><span class="info4">我的卡包</span></div>
      <div class="layer4 flex-col"></div>
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
        backTo(){
            this.$router.go(-1);
        },
        sealTo(){
            this.$router.push({
                path:'/',
                query:{
                    type:1
                }
            })
        }
    }
}
</script>

<style lang="scss" scoped>
html {
  font-size: 37.5px;
}
    .sealbuy{
        

.page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 102.4rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
  justify-content: flex-start;
  padding-top: 2.32rem;
  align-items: flex-start;
  padding-left: 2.454rem;
}

.pic1 {
  z-index: 3;
  width: 1.707rem;
  height: 3.094rem;
}

.layer1 {
  z-index: 2;
  position: absolute;
  left: -22.213rem;
  top: 6.454rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
    833px -32px no-repeat;
}

.layer2 {
  z-index: 6;
  height: 87.814rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 100px 20px rgba(0, 0, 0, 0.06);
  width: 48.214rem;
  justify-content: flex-end;
  padding-bottom: 4.054rem;
  align-items: center;
  position: absolute;
  left: 4.694rem;
  top: 9.254rem;
}

.wrap1 {
  z-index: auto;
  width: 44.054rem;
  height: 69.414rem;
}

.block1 {
  z-index: 14;
  height: 25.04rem;
  border-radius: 46px;
  overflow: hidden;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge0fec930f15174e0d8e2d03b19fcef7b61b2161415fcff46479f3816989a431b)
    100% no-repeat;
  align-self: center;
  width: 44.054rem;
  justify-content: flex-start;
  padding-top: 1.307rem;
  align-items: center;
  position: relative;
}

.group1 {
  z-index: 16;
  position: relative;
  width: 41.28rem;
  height: 4.48rem;
  border-radius: 27px;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng028cc787fecb2e91f600842dd1dee9edff89e8062c03d3fd71b94e2ce864c62d)
    100% no-repeat;
}

.info1 {
  z-index: 17;
  position: absolute;
  left: 0.694rem;
  top: 0.56rem;
  width: 39.894rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 0.88);
  font-size: 2.4rem;
  font-family: PingFangSC-Medium;
  line-height: 3.36rem;
  text-align: center;
}

.pic2 {
  z-index: 15;
  position: absolute;
  left: 0;
  top: 0;
  width: 44.054rem;
  height: 25.04rem;
}

.block2 {
  z-index: 28;
  width: 43.76rem;
  height: 0.054rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge82ef14b717a81ecc6e47ba6b90293cd21c81535e217ded0bfbfd64d59f5c0f7)
    100% no-repeat;
  align-self: center;
  margin-top: 20.64rem;
}

.img1 {
  z-index: 30;
  width: 3.174rem;
  height: 1.974rem;
  align-self: center;
  margin-top: 9.814rem;
}

.block3 {
  z-index: 18;
  position: relative;
  width: 23.2rem;
  height: 6.694rem;
  border-radius: 125.5px 125.5px 125.5px 125.5px;
  background-color: rgba(23, 88, 255, 1);
  align-self: center;
  margin-top: 5.2rem;
}

.word1 {
  z-index: 19;
  position: absolute;
  left: 4.774rem;
  top: 1.494rem;
  width: 13.68rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
}

.txt1 {
  z-index: 20;
  position: absolute;
  left: 20.907rem;
  top: 41.947rem;
  width: 6.4rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  line-height: 2.987rem;
  text-align: center;
}

.word2 {
  z-index: 21;
  position: absolute;
  left: 17.547rem;
  top: 44.934rem;
  width: 13.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 3.2rem;
  font-family: PingFangSC-Medium;
  line-height: 4.48rem;
  text-align: center;
}

.info2 {
  z-index: 24;
  position: absolute;
  left: 33.014rem;
  top: 52.454rem;
  width: 13.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: right;
}

.txt2 {
  z-index: 23;
  position: absolute;
  left: 17.547rem;
  top: 52.454rem;
  width: 13.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.word3 {
  z-index: 22;
  position: absolute;
  left: 2.08rem;
  top: 52.454rem;
  width: 13.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Medium;
  line-height: 2.614rem;
  text-align: center;
}

.word4 {
  z-index: 27;
  position: absolute;
  left: 32.32rem;
  top: 55.44rem;
  width: 12.427rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 0, 0, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: right;
}

.info3 {
  z-index: 26;
  position: absolute;
  left: 17.92rem;
  top: 55.44rem;
  width: 12.427rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 0, 0, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
}

.word5 {
  z-index: 25;
  position: absolute;
  left: 2.08rem;
  top: 55.44rem;
  width: 12.427rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 1, 1, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.word6 {
  z-index: 29;
  position: absolute;
  left: 2.8rem;
  top: 66.8rem;
  width: 42.614rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.layer3 {
  z-index: 7;
  position: absolute;
  left: 4.72rem;
  top: 9.254rem;
  width: 48.24rem;
  height: 8.16rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng3b25d146904e8865e69b7d3ad473997da35798b68e4ab42758744e18a6200f3b) -60px -59.5px
    no-repeat;
    background-size:117% auto;
}

.info4 {
  z-index: 12;
  position: absolute;
  left: 13.627rem;
  top: 2.08rem;
  width: 20.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Semibold;
  line-height: 3.734rem;
  text-align: center;
}

.layer4 {
  z-index: 5;
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