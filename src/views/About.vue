<template>
  <div class="page flex-col about">
      <div class="mod1 flex-col" :class="{'IndexbuyIng':buyIng == 1 || buyIng == 3 || hqShow}">
        <div class="outer1 flex-row">
          <img
            class="pic1"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngef02e9b613a1f326f904f6b0fe96cf8cf0cf5a3f7e50979d62b5ed7b4d8682ac"
            @click.stop="back"
          />
          <img
            class="pic2"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngba7ee175c4a17203d134d8066bfaeb2eab9a147796871dc6f009c2d4af9892ca"
             @click.stop="closeWindow"
          />
          <img
            class="pic3"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng3a001189a941b9f763f1afadfee5ace134dff4b7f9cd32aec907bcf1ccabadbf"
             @click.stop="openHome"
          />
        </div>
      </div>
      <div class="mod2 flex-col" :class="{'IndexMode':guide == 1}">
        <div class="outer2 flex-row">
          <div class="bd1 flex-col">
            <div class="outer3 flex-col">
              <img
                class="pic4"
                referrerpolicy="no-referrer"
                src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng27dba49fa8932e394f48bc154963648fcdb2da35fa25563f2800ac0350b13a50"
              />
            </div>
          </div>
        </div>
        <div class="outer4 flex-row">
          <!-- <div v-for="(item,index) in 7" v-bind:key="index">
            <div class="flex-col" :class="`section${mounth}`"></div>
          </div> -->
          <div class="section1 flex-col" :class="{sectioned:mounth == 1}"><span v-if="mounth == 1">1</span></div>
          <div class="section2 flex-col" :class="{sectioned:mounth == 2}"><span v-if="mounth == 2">2</span></div>
          <div class="section3 flex-col" :class="{sectioned:mounth == 3}"><span v-if="mounth == 3">3</span></div>
          <div class="section4 flex-col" :class="{sectioned:mounth == 4}"><span v-if="mounth == 4">4</span></div>
          <div class="section5 flex-col" :class="{sectioned:mounth == 5}"><span v-if="mounth == 5">5</span></div>
          <div class="section6 flex-col" :class="{sectioned:mounth == 6}"><span v-if="mounth == 6">6</span></div>
          <div class="section7 flex-col" :class="{sectioned:mounth == 7}"><span v-if="mounth == 7">7</span></div>
          <div class="section8 flex-col" :class="{sectioned:mounth == 8}"><span v-if="mounth == 8">8</span></div>
          <!-- <div class="section9 flex-col"></div>
          <div class="section10 flex-col"></div> -->
        </div>
        <span class="word1">+0%</span>
        <span class="info1">收益率</span>
        <span class="info2">总资产</span>
        <span class="word2">{{price}}</span>
        <!-- <span class="info3">{{this.mounth}}</span> -->
        <span class="info4">进度</span>
      </div>
      <div v-if="guide == 1" class="section10-1 flex-col"></div>
      <div v-if="guide == 2" class="group22 flex-col"></div>
      <div v-if="guide == 3" class="section13 flex-col"></div>
      <div v-if="guide > 0" class="section4-1 flex-col">
        <div class="section5-1 flex-row"><div class="group1-1 flex-col"></div></div>
        <div class="section6-1 flex-row">
          <div class="block3-1 flex-col"><span class="info2-1" @click.stop="setupNext">知道啦</span></div>
        </div>
        <span class="word3-1" v-if="guide == 1">在这里查看你的总资产、收益和进度</span>
        <span class="paragraph12" v-if="guide == 2">
          市场可以进行投资
          <br />
          可以自由选择投多少哦
        </span>
         <span class="infoBox13" v-if="guide == 3">
          在这里
          <br />
          可以看你买了什么
        </span>
        <span class="txt4-1">我已经知道了，跳过</span>
      </div>
      
      <div class="mod3 flex-col" :class="{'IndexMode':guide == 2}">
        <div class="group1 flex-row">
          <div class="bd2 flex-col" @click.stop="buy('制药')">
            <img
              class="img1"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2a43fa3b0b590dcf442c9176a03b2d9789f7a5d7079a833e06a7c7a3ed0782d5"
            />
            <span class="word3">制药</span>
          </div>
          <div class="bd3 flex-col" @click.stop="buy('金属')">
            <div class="mod4 flex-col"></div>
            <span class="txt1">金属</span>
          </div>
          <div class="bd4 flex-col" @click.stop="buy('房地产')">
            <img
              class="img2"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngd2d0a99f76f64a8516ef1c31fb6048596343bed2d514895b43101cd29caba26b"
            />
            <span class="word4">房地产</span>
          </div>
          <div class="bd5 flex-col" @click.stop="buy('新能源')">
            <div class="group2 flex-col"></div>
            <span class="word5">新能源</span>
          </div>
          <div class="bd6 flex-col" @click.stop="buy('半导体')">
            <div class="outer5 flex-col"></div>
            <span class="txt2">半导体</span>
          </div>
        </div>
        <span class="word6">商品市场</span>
      </div>
      <div class="mod5 flex-col"></div>
      <div class="mod6 flex-col" :class="{'IndexMode':guide == 3}">
        <span class="word7">当前持有</span>
        <span class="info5" v-if="buyIng<=1">您的仓库空空～</span>
        <div class="group7-7 flex-col">
          <div class="bd1-7 flex-row" v-if="buyIng == 2">
            <div class="outer1-7 flex-col">
              <div class="section2-7 flex-col">
                <div class="block2-7 flex-col"></div>
                <div class="block3-7 flex-col"></div>
              </div>
              <span class="info2-7">持有量：100</span>
              <span class="info3-7" @click.stop="sealOut">卖出</span>
            </div>
            <div class="outer2-7 flex-col"></div>
            <div class="outer3-7 flex-col"></div>
            <div class="outer4-7 flex-col"></div>
            <div class="outer5-7 flex-col"></div>
          </div>
        </div>
      </div>
      <div class="mod7 flex-col" :class="{'IndexMode':guide == 4}" @click.stop="hqShow = true">
        <div class="group3 flex-col"><span class="word8" @click.stop="newxMountd">下个月</span></div>
        <span class="word9">市场行情</span>
        <span class="word10">
          {{hqText}}
        </span>
      </div>
      <div class="block34 flex-col" v-if="guide == 4">
        <span class="word54" @click.stop="guide = 0">开始测试吧</span>
      </div>
      <div class="block14 flex-col" v-if="guide == 4"></div>
      <span class="infoBox14" v-if="guide == 4">
          这里可以看每个月的市场行情
          <br />
          在完成买入卖出操作后
          <br />
          点击“下个月”后
          <br />
          会刷新市场行情
      </span>
      <div class="mod8 flex-col"></div>
      <div class="main66 flex-col" v-if="closePrompt">
        <div class="main7 flex-col">
          <div class="layer1 flex-row">
            <div class="main8 flex-col"><span class="word3" @click.stop="closePrompt = false;">取消</span></div>
            <div class="main9 flex-col"><span class="word4" @click.stop="back">确定</span></div>
          </div>
          <span class="word5">您要结束测试吗？</span>
        </div>
      </div>
      <div class="group15 flex-col" v-if="buyIng == 1 || buyIng == 3">
        <div class="box3 flex-col">
          <div class="box4 flex-col">
            <div class="section1m flex-col">
              <div class="outer22 flex-col">
                <div class="group16 flex-col"></div>
                <span class="txt5">{{buyText}}</span>
                <span class="info5">单价：</span>
                <span class="word5">10.00</span>
              </div>
              <div class="outer3 flex-col">
                <span class="word6">1</span>
                <span class="word7">0</span>
                <span class="word8">0</span>
                <span class="info6">0</span>
              </div>
              <div class="outer4-8 flex-col"><span class="word9" @click.stop="buyChange">完成</span></div>
            </div>
            <span v-if="buyIng == 1" class="word10">买入金额</span>
            <span v-if="buyIng == 3" class="word10">卖出金额</span>
          </div>
          <img
            class="pic1"
            referrerpolicy="no-referrer"
            src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng7615e684a2c58a83a91cf6e04b76c98dbb5346b90f6549bd9c9e8583c44e739c"
          />
        </div>
        <span class="word11">请在下方取出金额</span>
      </div>
      <div class="wrap3-hq flex-col" v-if="hqShow">
        <div class="bd1-hq flex-col">
          <div class="layer1-hq flex-col">
            <div class="layer2-hq flex-col">
              <div class="mod3-hq flex-col">
                <div class="main1-hq flex-col"></div>
                <span class="txt4-hq">{{mounth == 2?'制药':'半导体'}}</span>
              </div>
              <div class="mod4-hq flex-col"></div>
              <div class="mod5-hq flex-col"></div>
              <div class="mod6-hq flex-col"></div>
              <div class="mod7-hq flex-col"></div>
              <div class="mod8-hq flex-col"></div>
            </div>
            <span class="word3-hq">20.00%</span>
            <div class="layer3-hq flex-col"></div>
            <span class="word4-hq">10.00%</span>
            <div class="layer4-hq flex-col"></div>
            <div class="layer5-hq flex-col"></div>
            <span class="word5-hq">0.00%</span>
            <span class="word6-hq">-10.00%</span>
            <span class="word7-hq">-20.00%</span>
            <span class="word8-hq">1月</span>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  data(){
    return{
      type:'',
      guide:1,
      mounth:1,
      price:10000,
      closePrompt:false,
      buyIng:0,
      buyText:'',
      hqText:'半导体利好的消息上热搜，大家纷纷抢购基金，但存在一定风险。',
      hqShow:false,
    }
  },
  created(){
    this.type = this.$route.query.type?this.$route.query.type:''
  },
  methods:{
    //1111
    setupNext(){
      this.guide++;
    },
    newxMountd(){
      if(this.guide<=0){
        this.mounth==8?this.mounth=1:this.mounth++
      }
      if(this.mounth == 2){
        this.hqText = '全球性流感来袭，制药行业成为热门投资板块，药价上涨。'
      }else{
        this.hqText = '半导体利好的消息上热搜，大家纷纷抢购基金，但存在一定风险。'
      }
      
    },
    back(){
      this.$router.go(-1);
    },
    closeWindow(){
      this.closePrompt = true;
    },
    buy(type){
      console.log(type)
      this.buyIng = 1;
      this.buyText = type;
    },
    buyChange(){
      if(this.buyIng == 1){
        this.buyIng = 2;
        this.price = 9000;
      }else{
        this.buyIng = 0;
        this.price = 10000;
      }
      
    },
    sealOut(){
      this.buyIng = 3;
    },
    openHome(){
      this.$router.push({path:'/',query:{type:1}})
    }
  }
}
</script>

<style lang="scss" scoped>
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
  justify-content: flex-end;
  padding-bottom: 2.907rem;
  align-items: center;
}
.about{
  .mod1 {
    z-index: 75;
    height: 9.414rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng69f824895abb95097ee4a597916d6d60fb44b4eab1f3094a491827d5ef91e7c6) 0 -30px
      no-repeat;
      background-size:100% auto;
    width: 38.427rem;
    justify-content: center;
    align-items: center;
  }

  .outer1 {
    z-index: auto;
    width: 28.587rem;
    height: 4.187rem;
    justify-content: space-between;
  }

  .pic1 {
    z-index: 82;
    width: 4.187rem;
    height: 4.187rem;
  }

  .pic2 {
    z-index: 86;
    width: 4.187rem;
    height: 4.187rem;
  }

  .pic3 {
    z-index: 78;
    width: 4.187rem;
    height: 4.187rem;
  }

  .mod2 {
    z-index: 2;
    height: 30.747rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng518a0fc4a1f098f24ff7a2d700f996e847a536bb0b69764853ba7ebaaad72bd2)
      100% no-repeat;
    background-size:100% auto;
    width: 63.68rem;
    position: absolute;
    left: -3.013rem;
    top: 0;
  }

  .outer2 {
    z-index: auto;
    width: 9.654rem;
    height: 9.654rem;
    margin: 79px 0 0 882.5px;
  }

  .bd1 {
    z-index: 60;
    height: 9.654rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng66394dd81ea202327a28c44a6a2fef1d47b4b0012d58e33595f2d1cafa6fd632)
      100% no-repeat;
      background-size:100% auto;
    width: 9.654rem;
    justify-content: center;
    align-items: center;
  }

  .outer3 {
    z-index: 91;
    position: relative;
    width: 8.64rem;
    height: 8.64rem;
    border-radius: 18px;
    overflow: hidden;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2948325c68dae44b4030e74c24f62643dfa05d7a54ee712c4747b8e458b3e7a3)
      100% no-repeat;
      background-size:100% auto;
  }

  .pic4 {
    z-index: 92;
    position: absolute;
    left: 0;
    top: 0;
    width: 8.64rem;
    height: 8.64rem;
  }

  .outer4 {
    z-index: auto;
    width: 31.334rem;
    height: 2.934rem;
    margin: 68.5px 0 0 487px;
  }

  .section1 {
    z-index: 63;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 21.5px;
  }

  .section2 {
    z-index: 65;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 21.5px;
  }

  .section3 {
    z-index: 66;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section4 {
    z-index: 67;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section5 {
    z-index: 68;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section6 {
    z-index: 69;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section7 {
    z-index: 70;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section8 {
    z-index: 71;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section9 {
    z-index: 72;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }

  .section10 {
    z-index: 73;
    width: 1.174rem;
    height: 1.174rem;
    background-color: rgba(69, 125, 254, 1);
    border-radius: 50%;
    margin: 18px 0 0 39px;
  }
  .sectioned{
    width: 2.934rem;
    height: 2.934rem;
    background-color: rgba(169, 195, 255, 1);
    margin: 0 0 0 21.5px;
    span{
      width:100%;
      height:100%;
      z-index:111;
      display:inline-block;
      color:#fff;
      font-size:2rem;
      line-height:1.5;
    }
  }
  .word1 {
    z-index: 59;
    position: absolute;
    left: 6.827rem;
    top: 16.827rem;
    width: 13.067rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: left;
  }

  .info1 {
    z-index: 57;
    position: absolute;
    left: 6.827rem;
    top: 13.574rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(162, 200, 253, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Medium;
    line-height: 2.987rem;
    text-align: left;
  }

  .info2 {
    z-index: 48;
    position: absolute;
    left: 6.854rem;
    top: 4.214rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(162, 200, 253, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Medium;
    line-height: 2.987rem;
    text-align: left;
  }

  .word2 {
    z-index: 50;
    position: absolute;
    left: 6.96rem;
    top: 7.2rem;
    width: 13.12rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: left;
  }

  .info3 {
    z-index: 64;
    position: absolute;
    left: 25.52rem;
    top: 17.307rem;
    width: 3.627rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.4rem;
    font-family: PingFangSC-Medium;
    line-height: 3.36rem;
    text-align: center;
  }

  .info4 {
    z-index: 58;
    position: absolute;
    left: 25.814rem;
    top: 13.574rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(162, 200, 253, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Medium;
    line-height: 2.987rem;
    text-align: left;
  }

  .mod3 {
    z-index: 7;
    height: 19.44rem;
    border-radius: 48px;
    background-color: rgba(255, 255, 255, 1);
    box-shadow: 0px 0px 50px 10px rgba(185, 185, 185, 0.2);
    width: 53.307rem;
    justify-content: flex-end;
    align-items: flex-end;
    position: absolute;
    left: 2.107rem;
    top: 23.2rem;
    padding: 0 32.5px 24.5px 0;
  }

  .group1 {
    z-index: auto;
    width: 49.76rem;
    height: 10.427rem;
    justify-content: space-between;
  }

  .bd2 {
    z-index: 13;
    height: 10.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
    width: 8.88rem;
    justify-content: flex-start;
    align-items: flex-end;
    position: relative;
    padding: 33px 45.5px 0 0;
  }

  .img1 {
    z-index: 20;
    width: 3.92rem;
    height: 3.174rem;
  }

  .word3 {
    z-index: 14;
    position: absolute;
    left: 1.307rem;
    top: 6.907rem;
    width: 6.24rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.6rem;
    font-family: PingFangSC-Regular;
    line-height: 2.24rem;
    text-align: center;
  }

  .bd3 {
    z-index: 9;
    height: 10.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
    width: 8.88rem;
    justify-content: flex-start;
    align-items: flex-end;
    position: relative;
    padding: 28.5px 39px 0 0;
  }

  .mod4 {
    z-index: 25;
    width: 4.454rem;
    height: 3.6rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng0f633feb254f1d730ba4275ff825d0c322fe259897ed90c14c816978abf337a6)
      0px 0px no-repeat;
      background-size:100% auto;
  }

  .txt1 {
    z-index: 15;
    position: absolute;
    left: 1.307rem;
    top: 6.907rem;
    width: 6.24rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.6rem;
    font-family: PingFangSC-Regular;
    line-height: 2.24rem;
    text-align: center;
  }

  .bd4 {
    z-index: 10;
    height: 10.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
    width: 8.88rem;
    justify-content: flex-start;
    padding-top: 1.494rem;
    align-items: center;
    position: relative;
  }

  .img2 {
    z-index: 93;
    width: 3.627rem;
    height: 3.627rem;
  }

  .word4 {
    z-index: 16;
    position: absolute;
    left: 1.307rem;
    top: 6.907rem;
    width: 6.24rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.6rem;
    font-family: PingFangSC-Regular;
    line-height: 2.24rem;
    text-align: center;
  }

  .bd5 {
    z-index: 11;
    height: 10.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
    width: 8.88rem;
    justify-content: flex-start;
    padding-top: 2.507rem;
    align-items: center;
    position: relative;
  }

  .group2 {
    z-index: 32;
    width: 3.734rem;
    height: 2.054rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng76ae62b194adf2e3a94e50423fedb228cc01f8ca07620b0ba945c9704a638eaf) -2.5px -2.5px
      no-repeat;
      background-size:100% auto;
  }

  .word5 {
    z-index: 17;
    position: absolute;
    left: 1.28rem;
    top: 6.907rem;
    width: 6.24rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.6rem;
    font-family: PingFangSC-Regular;
    line-height: 2.24rem;
    text-align: center;
  }

  .bd6 {
    z-index: 12;
    height: 10.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
    width: 8.88rem;
    justify-content: flex-start;
    align-items: flex-start;
    position: relative;
    padding: 49.5px 0 0 56px;
  }

  .outer5 {
    z-index: 37;
    width: 2.747rem;
    height: 3.574rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng42085cdd6175ae54e9ebaecd0729400bcdb5c73b76238804efadad7247d015ab) -2.5px -2px
      no-repeat;
      background-size:100% auto;
  }

  .txt2 {
    z-index: 18;
    position: absolute;
    left: 1.28rem;
    top: 6.88rem;
    width: 6.24rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.6rem;
    font-family: PingFangSC-Regular;
    line-height: 2.24rem;
    text-align: center;
  }

  .word6 {
    z-index: 52;
    position: absolute;
    left: 1.734rem;
    top: 2rem;
    width: 14.934rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }

  .mod5 {
    z-index: 6;
    position: absolute;
    left: -22.826rem;
    top: 34.214rem;
    width: 26.987rem;
    height: 27.307rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnga890d1a60155ace076854425fe3b325df2ef2f3f948825cf0eac19d8cd30a4d9)
      428px -9.5px no-repeat;
      background-size:100% auto;
  }

  .mod6 {
    z-index: 46;
    position: absolute;
    left: 2.16rem;
    top: 44.347rem;
    width: 53.307rem;
    height: 20.934rem;
    border-radius: 49px;
    background-color: rgba(255, 255, 255, 1);
    box-shadow: 0px 0px 50px 10px rgba(185, 185, 185, 0.2);
  }

  .word7 {
    z-index: 51;
    position: absolute;
    left: 1.44rem;
    top: 2.267rem;
    width: 14.934rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }

  .info5 {
    z-index: 49;
    position: absolute;
    left: 18.8rem;
    top: 10.32rem;
    width: 15.574rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(172, 172, 172, 1);
    font-size: 1.76rem;
    font-family: PingFangSC-Medium;
    line-height: 2.454rem;
    text-align: center;
  }

  .mod7 {
    z-index: 47;
    height: 21.387rem;
    border-radius: 60px;
    background-color: rgba(23, 88, 255, 1);
    box-shadow: 0px 0px 50px 10px rgba(185, 185, 185, 0.2);
    width: 53.307rem;
    justify-content: flex-end;
    align-items: flex-end;
    position: absolute;
    left: 2.16rem;
    top: 66.987rem;
    padding: 0 32.5px 36px 0;
  }

  .group3 {
    z-index: 54;
    position: relative;
    width: 16.16rem;
    height: 5.04rem;
    border-radius: 43.75px 43.75px 43.75px 43.75px;
    background-color: rgba(255, 255, 255, 1);
  }

  .word8 {
    z-index: 55;
    position: absolute;
    left: 4.854rem;
    top: 1.04rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 1.866rem;
    font-family: PingFangSC-Medium;
    line-height: 2.614rem;
    text-align: center;
  }

  .word9 {
    z-index: 53;
    position: absolute;
    left: 1.627rem;
    top: 2.134rem;
    width: 14.934rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }

  .word10 {
    z-index: 56;
    position: absolute;
    left: 1.707rem;
    top: 7.76rem;
    width: 49.84rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 1.866rem;
    font-family: PingFangSC-Medium;
    line-height: 2.614rem;
    text-align: left;
  }

  .mod8 {
    z-index: 5;
    position: absolute;
    left: 51.467rem;
    top: 68.027rem;
    width: 26.987rem;
    height: 27.307rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2576e4a9e101c98b49f05ddaf263229cec676dafd8b8244a131052f55b22854e) -59.5px -30px
      no-repeat;
      background-size:100% auto;
  }
  .section10-1 {
    z-index: 99;
    position: absolute;
    left: 7.6rem;
    top: 29.68rem;
    width: 2.774rem;
    height: 23.44rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2c00d9e23d5fa57c07b27bf1cdf018a7deb40e752142566ac1bcd9f915d3927e) -3px -1px
      no-repeat;
      background-size:100% auto;
  }
  .IndexMode{
    z-index:76;
  }
  .section4-1 {
    z-index: 75;
    height: 102.4rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng6f94f9e9c97fd1009c73e1c00896d328df90e050ca268b97a460c8659a56a100)
      100% no-repeat;
      background-size:100% auto;
    width: 57.547rem;
    position: absolute;
    left: 0;
    top: 0;
  }

  .section5-1 {
    z-index: auto;
    width: 0.027rem;
    height: 0.027rem;
    margin: 592px 0 0 207.5px;
  }

  .group1-1 {
    z-index: 98;
    width: 0.027rem;
    height: 0.027rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng956c678e3e4cea89015618a91f250ab5d8c809bd26f10108544b138794cc46d5)
      100% no-repeat;
      background-size:100% auto;
  }

  .section6-1 {
    z-index: auto;
    width: 23.894rem;
    height: 10.054rem;
    margin: 765px 0 0 316px;
  }

  .block3-1 {
    z-index: 102;
    position: relative;
    width: 23.894rem;
    height: 10.054rem;
    border-radius: 94.25px 94.25px 94.25px 94.25px;
    background-color: rgba(255, 255, 255, 1);
  }

  .info2-1 {
    z-index: 103;
    position: absolute;
    left: 7.574rem;
    top: 3.094rem;
    width: 8rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }

  .word3-1 {
    z-index: 100;
    position: absolute;
    left: 8.187rem;
    top: 53.92rem;
    width: 42.667rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }

  .txt4-1 {
    z-index: 104;
    position: absolute;
    left: 20.64rem;
    top: 84.987rem;
    width: 16.8rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(160, 160, 160, 1);
    font-size: 1.866rem;
    font-family: PingFangSC-Medium;
    line-height: 2.614rem;
    text-align: center;
  }
  .group22 {
    z-index: 101;
    position: absolute;
    left: 40.934rem;
    top: 42.427rem;
    width: 10.24rem;
    height: 12.8rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng0885370d07a1c13da043ff437a215f763bf79539754c9928a4055487d024af46)
      100% no-repeat;
      background-size:100% auto;
  }
  .paragraph12 {
    z-index: 103;
    position: absolute;
    left: 15.467rem;
    top: 53.44rem;
    width: 26.667rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }
  .section13 {
    z-index: 94;
    width: 8.267rem;
    height: 9.84rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge642628f4016478687139175859e6ff75acc8518d20251767f28aae48d6df9bb)
      100% no-repeat;
      background-size:100% auto;
    align-self: flex-start;
    margin-left: 5.68rem;
    position: absolute;
      top: 34rem;
      left: 3rem;
  }
  .infoBox13 {
    z-index: 102;
    position: absolute;
    left: 17.52rem;
    top: 28.88rem;
    width: 21.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }
  .block34 {
    z-index: 101;
    position: relative;
    width: 23.894rem;
    height: 10.054rem;
    border-radius: 188.5px 188.5px 188.5px 188.5px;
    background-color: rgba(255, 255, 255, 1);
    align-self: center;
    margin-top: 2.054rem;
  }

  .word54 {
    z-index: 102;
    position: absolute;
    left: 4.907rem;
    top: 3.094rem;
    width: 13.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }
  .infoBox14 {
    z-index: 94;
    position: absolute;
    left: 10.827rem;
    top: 48.907rem;
    width: 34.667rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }
  .block14 {
    z-index: 93;
    width: 7.28rem;
    height: 8.934rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng863144d36d68c803958e90ba07d096e2063a4a702f825cd3d4999744e77c5239)
      100% no-repeat;
      background-size:100% auto;
    align-self: flex-start;
    margin-left: 4.88rem;
    position:absolute;
    top:58rem;
    left:3rem;
  }
  .main66 {
    z-index: 200;
    height: 102.4rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2513f8809d976becb674d50917dc847ca02739c3a8945b21eaa639d6559bc39d)
      100% no-repeat;
      background-size:100% auto;
    width: 57.547rem;
    justify-content: flex-start;
    align-items: flex-end;
    position: absolute;
    left: 0;
    top: 0;
    padding: 435px 38.5px 0 0;
    .main7 {
    z-index: 98;
    height: 35.12rem;
    border-radius: 90px;
    background-color: rgba(255, 255, 255, 1);
    width: 53.334rem;
    justify-content: flex-end;
    padding-bottom: 2.454rem;
    align-items: center;
    position: relative;
  }

  .layer1 {
    z-index: auto;
    width: 42.667rem;
    height: 5.92rem;
    justify-content: space-between;
  }

  .main8 {
    z-index: 100;
    position: relative;
    width: 16.454rem;
    height: 5.92rem;
    border-radius: 111px;
    background-color: rgba(23, 88, 255, 1);
  }

  .word3 {
    z-index: 101;
    position: absolute;
    left: 3.68rem;
    top: 0.88rem;
    width: 8.987rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }

  .main9 {
    z-index: 103;
    position: relative;
    width: 16.454rem;
    height: 5.92rem;
    border-radius: 111px;
    background-color: rgba(186, 186, 186, 1);
  }

  .word4 {
    z-index: 105;
    position: absolute;
    left: 3.68rem;
    top: 0.88rem;
    width: 8.987rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }

  .word5 {
    z-index: 104;
    position: absolute;
    left: 5.28rem;
    top: 11.014rem;
    width: 42.72rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }

  }
  .group15 {
    z-index: 97;
    height: 102.4rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng0760e3c9864016047ab87f15af950572fa43e94d9a591d22d66e0556d610278b)
      100% no-repeat;
      background-size:100% auto;
    width: 57.574rem;
    justify-content: flex-end;
    align-items: flex-start;
    position: absolute;
    left: 0.027rem;
    top: 0;
    padding: 0 0 54.5px 38.5px;
    .box3 {
    z-index: auto;
    width: 53.334rem;
    height: 76.294rem;
  }

  .box4 {
    z-index: 99;
    height: 35.12rem;
    border-radius: 90px;
    background-color: rgba(255, 255, 255, 1);
    align-self: center;
    width: 53.334rem;
    justify-content: flex-start;
    padding-top: 1.734rem;
    align-items: center;
    position: relative;
  }

  .section1m {
    z-index: auto;
    width: 49.76rem;
    height: 30.934rem;
  }

  .outer22 {
    z-index: 101;
    height: 8.08rem;
    border-radius: 17.5px;
    background-color: rgba(235, 241, 255, 1);
    align-self: center;
    width: 49.76rem;
    justify-content: center;
    align-items: flex-start;
    padding-left: 1.734rem;
    position: relative;
  }

  .group16 {
    z-index: 106;
    width: 3.68rem;
    height: 4.72rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbb6c05e87b317b5f1f54fcd239805ab5f5e72c067e6b0be6801d29df9fd50aed) -5px -4px
      no-repeat;
      background-size:100% auto;
  }

  .txt5 {
    z-index: 105;
    position: absolute;
    left: 7.627rem;
    top: 2.16rem;
    width: 10.587rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }

  .info5 {
    z-index: 102;
    position: absolute;
    left: 32.667rem;
    top: 2.614rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Medium;
    line-height: 2.987rem;
    text-align: center;
  }

  .word5 {
    z-index: 103;
    position: absolute;
    left: 35.867rem;
    top: 1.867rem;
    width: 12.427rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: right;
  }

  .outer3 {
    z-index: 117;
    position: relative;
    width: 26.827rem;
    height: 7.2rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngff780ab1bf9a6f9456dc0ce770f9f1caaaafa13130c9e09ce1dbee56d644c796)
      100% no-repeat;
      background-size:100% auto;
    align-self: flex-start;
    margin: 120px 0 0 214px;
  }

  .word6 {
    z-index: 153;
    position: absolute;
    left: 6rem;
    top: 1.36rem;
    width: 3.627rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: center;
  }

  .word7 {
    z-index: 169;
    position: absolute;
    left: 11.654rem;
    top: 1.36rem;
    width: 3.627rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: center;
  }

  .word8 {
    z-index: 170;
    position: absolute;
    left: 17.254rem;
    top: 1.36rem;
    width: 3.627rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: center;
  }

  .info6 {
    z-index: 171;
    position: absolute;
    left: 22.8rem;
    top: 1.36rem;
    width: 3.627rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Medium;
    line-height: 4.48rem;
    text-align: center;
  }

  .outer4-8 {
    z-index: 151;
    position: relative;
    width: 16.454rem;
    height: 5.92rem;
    border-radius: 55.5px;
    background-color: rgba(23, 88, 255, 1);
    align-self: center;
    margin-top: 3.334rem;
  }

  .word9 {
    z-index: 152;
    position: absolute;
    left: 3.68rem;
    top: 0.88rem;
    width: 8.987rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }

  .word10 {
    z-index: 116;
    position: absolute;
    left: 19.894rem;
    top: 11.014rem;
    width: 13.467rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: center;
  }

  .pic1 {
    z-index: 125;
    width: 4.4rem;
    height: 3.92rem;
    align-self: flex-start;
    margin: 48px 0 0 261px;
  }

  .box5 {
    z-index: 154;
    width: 38.427rem;
    height: 9.414rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng031cda079c5c06d3ff74ed673e0f30545b40fabd4a76c7ee93a8ba06fdb32764) -120px -114px
      no-repeat;
      background-size:100% auto;
    align-self: flex-end;
    margin: 474px 138.5px 0 0;
  }

  .word11 {
    z-index: 124;
    position: absolute;
    left: 20.374rem;
    top: 61.36rem;
    width: 21.067rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Medium;
    line-height: 2.987rem;
    text-align: center;
  }

  }
  .IndexbuyIng{
    z-index:108;
  }


  .group7-7 {
    z-index: 35;
    height: 20.934rem;
    border-radius: 49px;
    background-color: rgba(255, 255, 255, 1);
    box-shadow: 0px 0px 100px 20px rgba(185, 185, 185, 0.2);
    width: 53.307rem;
    justify-content: flex-end;
    padding-bottom: 1.654rem;
    align-items: center;
    position: absolute;
    left: 0;
    top: 0;
  }


  .bd1-7 {
    z-index: auto;
    width: 49.76rem;
    height: 12.427rem;
    justify-content: space-between;
  }

  .outer1-7 {
    z-index: 42;
    height: 12.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
    width: 8.88rem;
    justify-content: flex-end;
    padding-bottom: 1.147rem;
    align-items: center;
    position: relative;
  }

  .section2-7 {
    z-index: auto;
    width: 6.4rem;
    height: 9.814rem;
  }

  .block2-7 {
    z-index: 43;
    width: 2.747rem;
    height: 3.574rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng42085cdd6175ae54e9ebaecd0729400bcdb5c73b76238804efadad7247d015ab) -5px -4px
      no-repeat;
      background-size:100% auto;
    align-self: center;
  }

  .block3-7 {
    z-index: 86;
    width: 6.4rem;
    height: 2.667rem;
    border-radius: 25px;
    background-color: rgba(23, 88, 255, 1);
    align-self: center;
    margin-top: 3.574rem;
  }

  .info2-7 {
    z-index: 88;
    position: absolute;
    left: 1.227rem;
    top: 5.347rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.12rem;
    font-family: PingFangSC-Medium;
    line-height: 1.574rem;
    text-align: center;
  }

  .info3-7 {
    z-index: 87;
    position: absolute;
    left: 1.2rem;
    top: 9.067rem;
    width: 6.4rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 1.28rem;
    font-family: PingFangSC-Medium;
    line-height: 1.787rem;
    text-align: center;
  }

  .outer2-7 {
    z-index: 38;
    width: 8.88rem;
    height: 12.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
  }

  .outer3-7 {
    z-index: 39;
    width: 8.88rem;
    height: 12.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
  }

  .outer4-7 {
    z-index: 40;
    width: 8.88rem;
    height: 12.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
  }

  .outer5-7 {
    z-index: 41;
    width: 8.88rem;
    height: 12.427rem;
    border-radius: 40.5px;
    background-color: rgba(108, 149, 255, 0.13);
  }

  .info4-7 {
    z-index: 52;
    position: absolute;
    left: 1.44rem;
    top: 2.267rem;
    width: 14.934rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }


  .wrap3-hq {
    z-index: 97;
    height: 102.4rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng0308c3ee384b7e25fab4f89d958c5fac2a288747f9aef4f03fcc5dbacade32bc)
      100% no-repeat;
      background-size:100% auto;
    width: 57.574rem;
    justify-content: flex-end;
    padding-bottom: 2.907rem;
    align-items: center;
    position: absolute;
    left: 0.054rem;
    top: 0;
  }

  .bd1-hq {
    z-index: auto;
    width: 53.334rem;
    height: 76.294rem;
  }

  .layer1-hq {
    z-index: 113;
    height: 35.12rem;
    border-radius: 90px;
    background-color: rgba(255, 255, 255, 1);
    align-self: center;
    width: 53.334rem;
    justify-content: flex-start;
    padding-top: 1.734rem;
    align-items: center;
    position: relative;
  }

  .layer2-hq {
    z-index: auto;
    width: 49.76rem;
    height: 28.24rem;
  }

  .mod3-hq {
    z-index: 114;
    height: 8.08rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngf94bbcbfaef76d940a339499ebde32661f47ec4687224d02539bea7573fa6864)
      100% no-repeat;
      background-size:100% auto;
    align-self: center;
    width: 49.76rem;
    justify-content: center;
    align-items: flex-start;
    padding-left: 1.707rem;
    position: relative;
  }

  .main1-hq {
    z-index: 118;
    width: 3.68rem;
    height: 4.72rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbb6c05e87b317b5f1f54fcd239805ab5f5e72c067e6b0be6801d29df9fd50aed) -5px -4px
      no-repeat;
      background-size:100% auto;
  }

  .txt4-hq {
    z-index: 117;
    position: absolute;
    left: 7.6rem;
    top: 2.16rem;
    width: 10.587rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 2.666rem;
    font-family: PingFangSC-Medium;
    line-height: 3.734rem;
    text-align: left;
  }

  .mod4-hq {
    z-index: 139;
    width: 45.227rem;
    height: 0.054rem;
    border: 1px solid rgba(151, 151, 151, 1);
    align-self: flex-end;
    margin: 65px 4.5px 0 0;
  }

  .mod5-hq {
    z-index: 138;
    width: 45.227rem;
    height: 0.054rem;
    border: 1px solid rgba(151, 151, 151, 1);
    align-self: flex-end;
    margin: 77px 4.5px 0 0;
  }

  .mod6-hq {
    z-index: 137;
    width: 45.227rem;
    height: 0.054rem;
    border: 1px solid rgba(151, 151, 151, 1);
    align-self: flex-end;
    margin: 77px 4.5px 0 0;
  }

  .mod7-hq {
    z-index: 136;
    width: 45.227rem;
    height: 0.054rem;
    border: 1px solid rgba(151, 151, 151, 1);
    align-self: flex-end;
    margin: 77px 4.5px 0 0;
  }

  .mod8-hq {
    z-index: 135;
    width: 45.227rem;
    height: 0.054rem;
    border: 1px solid rgba(151, 151, 151, 1);
    align-self: flex-end;
    margin: 77px 4.5px 0 0;
  }

  .word3-hq {
    z-index: 128;
    position: absolute;
    left: 2.107rem;
    top: 12.64rem;
    width: 4.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 0.96rem;
    font-family: PingFangSC-Medium;
    line-height: 1.334rem;
    text-align: left;
  }

  .layer3-hq {
    z-index: 142;
    position: absolute;
    left: 15.28rem;
    top: 16.187rem;
    width: 1.467rem;
    height: 1.467rem;
    background-color: rgba(0, 145, 255, 1);
    border-radius: 50%;
  }

  .word4-hq {
    z-index: 129;
    position: absolute;
    left: 2.08rem;
    top: 16.8rem;
    width: 4.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 0.96rem;
    font-family: PingFangSC-Medium;
    line-height: 1.334rem;
    text-align: left;
  }

  .layer4-hq {
    z-index: 140;
    position: absolute;
    left: 6.08rem;
    top: 16.907rem;
    width: 9.92rem;
    height: 4.72rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng55028993d7e6cacb426b09d2c91b299c9ba8063e66e036af1466b5f09555ba50) -3px -6px
      no-repeat;
      background-size:100% auto;
  }

  .layer5-hq {
    z-index: 141;
    position: absolute;
    left: 5.36rem;
    top: 20.88rem;
    width: 1.467rem;
    height: 1.467rem;
    background-color: rgba(0, 145, 255, 1);
    border-radius: 50%;
  }

  .word5-hq {
    z-index: 133;
    position: absolute;
    left: 2.08rem;
    top: 20.987rem;
    width: 4.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 0.96rem;
    font-family: PingFangSC-Medium;
    line-height: 1.334rem;
    text-align: left;
  }

  .word6-hq {
    z-index: 130;
    position: absolute;
    left: 1.974rem;
    top: 25.147rem;
    width: 4.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 0.96rem;
    font-family: PingFangSC-Medium;
    line-height: 1.334rem;
    text-align: left;
  }

  .word7-hq {
    z-index: 131;
    position: absolute;
    left: 1.974rem;
    top: 29.334rem;
    width: 4.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 0.96rem;
    font-family: PingFangSC-Medium;
    line-height: 1.334rem;
    text-align: left;
  }

  .word8-hq {
    z-index: 132;
    position: absolute;
    left: 13.867rem;
    top: 31.147rem;
    width: 4.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(109, 114, 120, 1);
    font-size: 0.96rem;
    font-family: PingFangSC-Medium;
    line-height: 1.334rem;
    text-align: center;
  }

  .layer6-hq {
    z-index: 98;
    width: 38.427rem;
    height: 9.414rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng031cda079c5c06d3ff74ed673e0f30545b40fabd4a76c7ee93a8ba06fdb32764) -120px -114px
      no-repeat;
      background-size:100% auto;
    align-self: flex-start;
    margin: 595.5px 0 0 139px;
  }




}



</style>