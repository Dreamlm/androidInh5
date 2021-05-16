<template>
  <div class="mycard">
      <div class="page flex-col">
      <img
        @click.stop="backTo"
        class="img1"
        referrerpolicy="no-referrer"
        src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbaee696ebb27ebb019468d44c8ac7bcabe494e65c8fab569c6560fcd63f4aec0"
      />
      <div class="box1 flex-col"></div>
      <div class="box2 flex-col">
        <div class="group1 flex-col">
          <div class="wrap1 flex-col">
            <div class="bd1 flex-col">
              <span class="word1">8462&nbsp;8383&nbsp;1988&nbsp;4282</span>
            </div>
            <img
                @click.stop="toSeal"
              class="img2"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng25ec67b6892fd855ee3c6ba6fe9765e3ec5de648ab21e0905856ecb925e00dbd"
            />
          </div>
          <div class="wrap2 flex-col"></div>
          <div class="wrap3 flex-col"><span class="word2" @click.stop="sealBuy">继续购买</span></div>
        </div>
      </div>
      <div class="box3 flex-col"><span class="word3">我的卡包</span></div>
      <div class="box4 flex-col"></div>
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
        sealBuy(){
            this.$router.push({
                path:'/entry'
            })
        },
        toSeal(){
            this.$router.push({
                path:'/sealbuy'
            })
        }
    }
}
</script>

<style lang="scss" scoped>
html {
  font-size: 18.75px;
}
    .mycard{
        

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

.img1 {
  z-index: 3;
  width: 1.707rem;
  height: 3.094rem;
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

.group1 {
  z-index: auto;
  width: 44.054rem;
  height: 69.414rem;
}

.wrap1 {
  z-index: 14;
  height: 14.16rem;
  border-radius: 46px;
  overflow: hidden;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnga9d5f97dec743daa79c2b7d236da814e8c295c7c125389d04ae8307024112a52)
    100% no-repeat;
  align-self: center;
  width: 44.054rem;
  justify-content: flex-start;
  padding-top: 1.307rem;
  align-items: center;
  position: relative;
}

.bd1 {
  z-index: 16;
  position: relative;
  width: 41.28rem;
  height: 4.48rem;
  border-radius: 27px;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng028cc787fecb2e91f600842dd1dee9edff89e8062c03d3fd71b94e2ce864c62d)
    100% no-repeat;
}

.word1 {
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

.img2 {
  z-index: 15;
  position: absolute;
  left: 0;
  top: 0;
  width: 44.054rem;
  height: 14.16rem;
}

.wrap2 {
  z-index: 20;
  width: 43.76rem;
  height: 0.054rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngcb7d7f642ca58f4c098bb2b099a57e3553fdfdd2d6534d99be6759ba5191677a)
    0px 0px no-repeat;
    background-size:100% auto;
  align-self: center;
  margin-top: 2.507rem;
}

.wrap3 {
  z-index: 18;
  position: relative;
  width: 23.2rem;
  height: 6.694rem;
  border-radius: 125.5px 125.5px 125.5px 125.5px;
  background-color: rgba(23, 88, 255, 1);
  align-self: center;
  margin-top: 46rem;
}

.word2 {
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

.box3 {
  z-index: 7;
  position: absolute;
  left: 4.72rem;
  top: 9.254rem;
  width: 48.24rem;
  height: 8.16rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng3b25d146904e8865e69b7d3ad473997da35798b68e4ab42758744e18a6200f3b) -62px -59.5px
    no-repeat;
    background-size:117% auto;
}

.word3 {
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

.box4 {
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