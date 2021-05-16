<template>
  <div class="cart">
    <div class="page flex-col">
      <div class="mod1 flex-col"></div>
      <div class="mod2 flex-col">
        <div class="wrap1 flex-col">
          <div class="main1 flex-col"></div>
          <div class="swiper-container">
            <div class="swiper-wrapper">
              <div
                v-for="(item, i) in 6"
                :key="i"
                class="swiper-slide"
              >
                <img
                    width="100"
                    class="pic1"
                    referrerpolicy="no-referrer"
                    src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngfd6b35795dfac9537ba2013425943cf3af728dbfa7d5670be43b5920546437b3"
                  />
              </div>
            </div>
            <div class="swiper-pagination"></div>
            <div class="investproTab investpro-prev swiper-button-prev" id="investpro-prev" @click.stop="prev(1)"></div>
            <div class="investproTab investpro-next swiper-button-next" id="investpro-next" @click.stop="prev(2)"></div>
          </div>
        </div>
        <span class="word1">自定义外观</span>
        <div class="wrap2 flex-col"></div>
        <img
          class="img3"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngfde37e5929c59a01a4450deb01edda1563537c3a4d30d09cb507b112c72feeeb"
        />
        <img
          class="pic3"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngef15d6cc049821127d03c200bc43e161f7cf26da2b6092b5255376aaf57f8886"
        />
      </div>
      <div class="mod3 flex-col">
        <div class="section1 flex-col"><span class="txt1" @click.stop="toMyCard">选择</span></div>
      </div>
      <div class="mod4 flex-col">
        <div class="block1 flex-col"></div>
        <span class="word2">锐意进取策略</span>
        <span class="word3">中高风险</span>
        <span class="txt2">转入金额</span>
        <span class="word4">交易规则</span>
        <span class="txt3">￥</span>
        <span class="info1">100.00元起购</span>
        <span class="word5">8000元</span>
        <span class="word6">6000元</span>
        <span class="word7">5000元</span>
        <span class="paragraph1">
          确认时间：现在转入，预计04月14日（星期三）24点前确认份额。
          <br />
          转入费率：基金交易相关费用按照基金产品收费规则收取。
        </span>
        <span class="txt4">扫码立即转入</span>
        <span class="word8">
          请在下方展示付款码进行交易，您将获取一张实体理财卡，请注意保存，市场有风险，投资需谨慎。
        </span>
      </div>
      <div class="mod5 flex-col"></div>
    </div>
  </div>
</template>

<script>
import Swiper from 'swiper';
export default {
  data(){
    return{
      swiper:{}
    }
  },
  mounted(){
    this.swiper = new Swiper('.swiper-container',{
      direction: 'horizontal',
      loop: true,
      autoplay: false,
      slidesPerView: "auto",
      centeredSlides:true,
      spaceBetween: 80,
      nextButton: '.swiper-button-next',
      prevButton: '.swiper-button-prev',
      // 如果需要分页器
      pagination: {
        el:'.swiper-pagination',
        clickable:true
      },
      
    })
  },
  methods:{
    prev(type){
      console.log(type)
      if(type == 1){
        this.swiper.slidePrev()
      }else{
        this.swiper.slideNext()
      }
    },
    toMyCard(){
      this.$router.push({path:'/mycard'})
    }
  }
}
</script>

<style lang="scss">
html{
  font-size:18.75px;
}
.cart{
  width:1080px;
  overflow:hidden;
  margin:0 auto;
  .page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 102.4rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
}

.mod1 {
  z-index: 2;
  position: absolute;
  left: -22.213rem;
  top: 6.454rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
    416px -16px no-repeat;
    background-size:100% auto;
}

.mod2 {
  z-index: 39;
  height: 74.987rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 25px 5px rgba(0, 0, 0, 0.06);
  width: 69.6rem;
  justify-content: flex-start;
  align-items: flex-start;
  position: absolute;
  left: -3.306rem;
  top: 8.534rem;
  padding: 152px 0 0 62px;
}

.wrap1 {
  z-index: auto;
  width: 57.6rem;
  height: 57.014rem;
}

.main1 {
  z-index: 43;
  width: 51.28rem;
  height: 0.054rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng32daec65f40bce451651a61ada747c662ee71ddb4615346ca26fdb66295b03e6)
    100% no-repeat;
    background-size:100% auto;
  align-self: center;
}

.main2 {
  z-index: auto;
  width: 57.6rem;
  height: 43.227rem;
  margin-top: 7.734rem;
  justify-content: space-between;
}

.box1 {
  z-index: 51;
  position: relative;
  width: 11.52rem;
  height: 43.227rem;
  border-radius: 42px;
  overflow: hidden;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng0ddd033b350aa3242125eebab5de75d0f36bb0c694fd90d34e318b04e6ddf6c4)
    100% no-repeat;
    background-size:100% auto;
}

.img1 {
  z-index: 52;
  position: absolute;
  left: 0;
  top: 0;
  width: 11.52rem;
  height: 43.227rem;
}

.box2 {
  z-index: 45;
  position: relative;
  width: 28.72rem;
  height: 43.227rem;
  border-radius: 42px;
  overflow: hidden;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge40e0a888c58553c90ee2fa7a4d145f47fb15d07d3668776b43bb9f3dc974a80)
    100% no-repeat;
    background-size:100% auto;
}

.pic1 {
  z-index: 46;
  position: absolute;
  left: 0;
  top: 0.054rem;
  width: 28.72rem;
  height: 43.094rem;
}

.box3 {
  z-index: 48;
  position: relative;
  width: 11.574rem;
  height: 43.094rem;
  border-radius: 42px;
  overflow: hidden;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng54035f08491b3c8a516dd3a50056db4c5448b8d692297f0b41a81c1d9e86b6b1)
    100% no-repeat;
    background-size:100% auto;
}

.pic2 {
  z-index: 49;
  position: absolute;
  left: 0;
  top: 0;
  width: 11.574rem;
  height: 43.094rem;
}

.img2 {
  z-index: 57;
  width: 12.454rem;
  height: 1.254rem;
  align-self: center;
  margin-top: 4.747rem;
}

.word1 {
  z-index: 42;
  position: absolute;
  left: 15.2rem;
  top: 2rem;
  width: 34.027rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 3.733rem;
  font-family: PingFangSC-Medium;
  line-height: 5.227rem;
  text-align: center;
}

.wrap2 {
  z-index: 56;
  position: absolute;
  left: 16.374rem;
  top: 14.587rem;
  width: 31.44rem;
  height: 46.054rem;
  border-radius: 51.5px;
  border: 12px solid rgba(23, 88, 255, 1);
}

.img3 {
  z-index: 53;
  position: absolute;
  left: 4.374rem;
  top: 35.867rem;
  width: 55.467rem;
  height: 5.067rem;
}

.pic3 {
  z-index: 64;
  position: absolute;
  left: 5.92rem;
  top: 36.854rem;
  width: 52.4rem;
  height: 3.094rem;
}

.mod3 {
  z-index: 38;
  height: 102.4rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6448999ae7ccf0fcc2b6b14ac883fb7edfcffeaff3c967aab05fd28aea8afc97)
    100% no-repeat;
    background-size:100% auto;
  width: 57.6rem;
  justify-content: flex-end;
  align-items: flex-end;
  position: absolute;
  left: 0;
  top: 0;
  padding: 0 363.5px 160px 0;
}

.section1 {
  z-index: 40;
  position: relative;
  width: 18.587rem;
  height: 6.694rem;
  border-radius: 62.75px 62.75px 62.75px 62.75px;
  background-color: rgba(23, 88, 255, 1);
}

.txt1 {
  z-index: 41;
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

.mod4 {
  z-index: 4;
  height: 87.814rem;
  border-radius: 68px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 50px 10px rgba(0, 0, 0, 0.06);
  width: 48.214rem;
  justify-content: flex-end;
  padding-bottom: 2.854rem;
  align-items: center;
  position: absolute;
  left: 4.694rem;
  top: 9.254rem;
}

.block1 {
  z-index: 27;
  width: 19.947rem;
  height: 13.974rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng8270a479f80bf68f4ae19222a140acf9ad810ed3b05b33dd8e773f54818f416c)
    100% no-repeat;
    background-size:100% auto;
}

.word2 {
  z-index: 11;
  position: absolute;
  left: 13.707rem;
  top: 0.987rem;
  width: 20.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(191, 80, 29, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Semibold;
  line-height: 3.734rem;
  text-align: center;
}

.word3 {
  z-index: 10;
  position: absolute;
  left: 20.694rem;
  top: 4.987rem;
  width: 6.907rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(191, 80, 29, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Regular;
  line-height: 2.24rem;
  text-align: center;
}

.txt2 {
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

.word4 {
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

.txt3 {
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

.info1 {
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

.word5 {
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

.word6 {
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

.txt4 {
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

.word8 {
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

.mod5 {
  z-index: 3;
  position: absolute;
  left: 51.414rem;
  top: 69.307rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6e7aff12b40a4794584456e61a45b32447c004658913bbafa7ba097d46d7abda) -59.5px -30px
    no-repeat;
    background-size:100% auto;
}
}
.swiper-container {
    margin-top: 8rem;
    width: 100%;
    overflow: visible!important;
    z-index:65;
}
.swiper-container .swiper-wrapper .swiper-slide{ width: 28.44rem; border-radius: 20px;}
.swiper-container .swiper-wrapper .swiper-slide img{width: 100%;  border-radius: 20px;}
.swiper-container .swiper-wrapper .swiper-slide-prev{ margin-top: 18px; height: 43.094rem important;}
.swiper-container .swiper-wrapper .swiper-slide-next{ margin-top: 18px;}
.swiper-container .swiper-wrapper .swiper-slide-active{ width: 28.44rem;}

.swiper-pagination{
    bottom: -30px!important;
}
.swiper-pagination .swiper-pagination-bullet{width: 12px; height: 12px; background: #ff1e1e;}
.swiper-pagination .swiper-pagination-bullet-active{width: 21px; height: 12px; background: #e75230; border-radius: 6px;}
.investproTab{width:5rem;height:5rem;border-radius:50%;z-index:65;background:url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngef15d6cc049821127d03c200bc43e161f7cf26da2b6092b5255376aaf57f8886) left center no-repeat;background:auto 5rem;position:absolute;left:0;top:20.6rem;left:1.1rem;}
.investpro-next{right:1.1rem;left:auto;background:url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngef15d6cc049821127d03c200bc43e161f7cf26da2b6092b5255376aaf57f8886) right center no-repeat;}
</style>
