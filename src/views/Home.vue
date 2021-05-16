<template>
  <div class="page flex-col home">
    <!-- <div class="main1 flex-row"><div class="wrap1 flex-col"></div></div>
    <div class="main2 flex-row"><div class="bd1 flex-col"></div></div>
    <div class="main3 flex-row">
      <img
        class="img1"
        referrerpolicy="no-referrer"
        src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge91eda90c89adfa509004ae2ede4e8052e3cad4f5038c95b6a4e2a4c1b5c4198"
      />
    </div>
    <div class="main4 flex-row"><div class="main5 flex-col"></div></div>
    <div class="main6 flex-row"><div class="box1 flex-col"></div></div>
    <div class="main7 flex-row">
      <img
        class="img2"
        referrerpolicy="no-referrer"
        src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngaf66f688cb51e18633b458b01ffa321613ca18e77e78258b534b36c63b18fb05"
      />
    </div> -->
    <div class="main8 flex-col" v-if="!type"><span class="info1c" @click.stop="start = true">进入测试</span></div>
    <div v-if="type" class="outer8-t flex-col" @click.stop="openLink(1)"><span class="word1-t">交易板块</span></div>
    <div v-if="type" class="outer9-t flex-col" @click.stop="openLink(0)"><span class="word2-t">返回首页</span></div>
    <!-- <img
      class="pic1"
      referrerpolicy="no-referrer"
      src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngd1134d30ab03b5cfb32c546d268aeb619386f7f0727e76e08cf380827992d8d1"
    /> -->
    <div class="outer3 flex-row" v-if="start">
        <!-- <div class="group1 flex-col"></div> -->
        <div v-if="!type" class="group2 flex-col"><span class="info1" @click.stop="openAbout">开始</span></div>
        <div v-if="type" class="group2 flex-col"><span class="info1" @click.stop="openAbout">确认</span></div>
      </div>
    <div class="outer5 flex-col" v-if="start">
      <div class="group3 flex-col">
        <div class="main1 flex-col"></div>
        <img
          class="img2"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnga10efe7d9bf4fc6f7bf9c2e545a146076cff1381c941c8b204c5c9033f5476b4"
        />
      </div>
      <span v-if="!type" class="word1">帮你了解自己的理财性格</span>
      <span v-if="!type" class="word2">您有&nbsp;8&nbsp;次决策机会，请谨慎选择</span>
      <span v-if="!type" class="word3">测试场景为虚拟场景，不构成建议，投资需谨慎。</span>
      <span v-if="type" class="word1">市场有风险，投资需谨慎哦～</span>
      <span v-if="type" class="word2">购买理财卡，长期持有稳定追求高回报</span>
      <span v-if="type" class="word3">内部收益数据仅供参考，过往业绩不代表未来表现，市场有风险，投资需谨慎。</span>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  data(){
    return{
      type:'',
      start:false
    }
  },
  created(){
    this.type = this.$route.query.type?this.$route.query.type:''
  },
  methods:{
    openAbout(){
      if(this.type){
        this.$router.push({path:'/user'});
      }else{
        this.$router.push({path:'/about'});
      }
    },
    openLink(type){
      if(type){
        this.start = true;
      }else{
        this.$router.push({path:'/'})
        this.type = '';
      }
    }
  }

}
</script>
<style lang="scss">
html {
  font-size: 18.75px;
}
.home{
  background: url(../assets/bg.png) repeat;
  background-size:100% auto;
  .main1 {
  z-index: auto;
  width: 10.934rem;
  height: 11.04rem;
  // margin: 812.5px 0 0 80px;
}

.wrap1 {
  z-index: 2;
  width: 10.934rem;
  height: 11.04rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng93639defe23dc7c6c5f817ec69283f214925b83267e86bc7ba58813a7d69dea2) -40px -39.5px
    no-repeat;
  background-size:100% auto;
}

.main2 {
  z-index: auto;
  width: 7.627rem;
  height: 7.734rem;
  margin: 442.5px 0 0 85.5px;
}

.bd1 {
  z-index: 5;
  width: 7.627rem;
  height: 7.734rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng5f35636ae9ff45c47cfb5055fd84d0f4a7b70bcc947c403d116828e0cc1af8da) -58.5px -58.5px
    no-repeat;
}

.main3 {
  z-index: auto;
  width: 12.347rem;
  height: 12rem;
  margin: -1496px 0 0 145px;
}

.img1 {
  z-index: 11;
  width: 12.347rem;
  height: 12rem;
}

.main4 {
  z-index: auto;
  width: 16.294rem;
  height: 16.507rem;
  margin: 1400px 0 0 1184px;
}

.main5 {
  z-index: 3;
  width: 16.294rem;
  height: 16.507rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6341ec4ff4c7dbcbfea1a940e4f900d03f7b5d08fdd56a09da88a3dac6a1cdfb) -59.5px -59.5px
    no-repeat;
    background-size:100% auto;
}

.main6 {
  z-index: auto;
  width: 12.667rem;
  height: 12.827rem;
  margin: -1551px 0 0 1320px;
}

.box1 {
  z-index: 4;
  width: 12.667rem;
  height: 12.827rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng42e9537c044478b5c5ad49d5b86459c53abc4e0c952b21db87d192e0150e0c16) -58.5px -59.5px
    no-repeat;
    background-size:100% auto;
}

.main7 {
  z-index: auto;
  width: 14.827rem;
  height: 14.347rem;
  margin: 840.5px 0 0 730.5px;
}

.img2 {
  z-index: 10;
  width: 14.827rem;
  height: 14.347rem;
}

.main8 {
  z-index: 7;
  position: absolute;
  left: 11.814rem;
  top: 46.48rem;
  width: 34rem;
  height: 9.414rem;
  border-radius: 88.25px 88.25px 88.25px 88.25px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 3px 50px 10px rgba(114, 79, 204, 0.2);
}

.info1c {
  z-index: 8;
  position: absolute;
  left: 8.854rem;
  top: 1.6rem;
  width: 16.294rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 4rem;
  font-family: PingFangSC-Medium;
  line-height: 5.6rem;
  text-align: center;
}

.pic1 {
  z-index: 9;
  position: absolute;
  left: 46.427rem;
  top: 42.187rem;
  width: 11.174rem;
  height: 12.24rem;
}

.outer5 {
  z-index: 9;
  height: 54.72rem;
  border-radius: 88.25px 88.25px 88.25px 88.25px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 50px 10px rgba(19, 118, 251, 0.12);
  width: 42.16rem;
  justify-content: flex-start;
  align-items: flex-start;
  position: absolute;
  left: 8.374rem;
  top: 17.04rem;
  padding: 151px 0 0 92px;
}

.group3 {
  z-index: auto;
  width: 30.134rem;
  height: 21.787rem;
}

.main1 {
  z-index: 13;
  width: 27.92rem;
  height: 10rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng5b80341fb23e014b3f0d5f75233ff1cc09f648b8fa56b0cbbd69665425120f4b)
    100% no-repeat;
  background-size:100% auto;
  align-self: flex-end;
}

.img2 {
  z-index: 12;
  width: 15.414rem;
  height: 10.774rem;
  align-self: flex-start;
  margin-top: 1.014rem;
}

.word1 {
  z-index: 14;
  position: absolute;
  left: 2.507rem;
  top: 11.12rem;
  width: 37.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 1.866rem;
  font-family: PingFangSC-Semibold;
  line-height: 2.614rem;
  text-align: center;
}

.word2 {
  z-index: 10;
  position: absolute;
  left: 2.507rem;
  top: 42.934rem;
  width: 37.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 2.133rem;
  font-family: PingFangSC-Semibold;
  line-height: 2.987rem;
  text-align: center;
}

.word3 {
  z-index: 11;
  position: absolute;
  left: 2.507rem;
  top: 47.867rem;
  width: 37.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(172, 172, 172, 1);
  font-size: 1.6rem;
  font-family: PingFangSC-Medium;
  line-height: 2.24rem;
  text-align: center;
}
.outer3 {
  z-index: auto;
  width: 100%;
  height: 9.227rem;
  justify-content: center;
  margin: 1420px 0 0 0px;
}

.group1 {
  z-index: 4;
  width: 7.627rem;
  height: 7.734rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng5f35636ae9ff45c47cfb5055fd84d0f4a7b70bcc947c403d116828e0cc1af8da) -58.5px 58.5px
    no-repeat;
  margin-top: 1.494rem;
}
.group2 {
  z-index: 15;
  position: relative;
  width: 18.587rem;
  height: 6.694rem;
  border-radius: 125.5px 125.5px 125.5px 125.5px;
  background-color: rgba(23, 88, 255, 1);
}

.info1 {
  z-index: 16;
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
}
.page {
  z-index: 1;
  position: relative;
  width: 57.6rem;
  height: 102.4rem;
  background-color: rgba(244, 245, 246, 1);
  overflow: hidden;
}


.outer8-t {
  z-index: 1;
  position: absolute;
  left: 11.814rem;
  top: 32.24rem;
  width: 34rem;
  height: 9.414rem;
  border-radius: 88.25px 88.25px 88.25px 88.25px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 3px 50px 10px rgba(114, 79, 204, 0.2);
}

.word1-t {
  z-index: 11;
  position: absolute;
  left: 8.854rem;
  top: 1.6rem;
  width: 16.294rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 4rem;
  font-family: PingFangSC-Medium;
  line-height: 5.6rem;
  text-align: center;
}

.outer9-t {
  z-index: 1;
  position: absolute;
  left: 11.814rem;
  top: 60.774rem;
  width: 34rem;
  height: 9.414rem;
  border-radius: 88.25px 88.25px 88.25px 88.25px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 3px 50px 10px rgba(114, 79, 204, 0.2);
}

.word2-t {
  z-index: 14;
  position: absolute;
  left: 8.854rem;
  top: 1.6rem;
  width: 16.294rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 4rem;
  font-family: PingFangSC-Medium;
  line-height: 5.6rem;
  text-align: center;
}



</style>
