<template>
  <div class="page flex-col">
      <div class="no-info" v-if="!info">
          <div class="layer1 flex-row">
        <div class="layer2 flex-col">
          <div class="bd1 flex-col">
            <img
                @click.stop="toCard"
              class="img1"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngeb0191ebf639f90e1d7108ac9610a1755afdaa291e25b2d73194c5c6c777a9a4"
            />
          </div>
        </div>
      </div>
      <div class="layer3 flex-row">
        <img
          class="img2"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng39a62907be9cdc480b11f13677ab863d6f0472a0c170dffe012e427cb10965e2"
        />
        <div class="section1">
          <span class="word1">Li，</span>
          <span class="word2">您好！</span>
        </div>
      </div>
      <div class="layer4 flex-col"></div>
      <div class="layer5 flex-col" @click.stop="info = true">
        <div class="block1 flex-col">
          <div class="main1 flex-row">
            <div class="section2 flex-col"></div>
          </div>
          <div class="main2 flex-row"><div class="bd2 flex-col"></div></div>
          <div class="main3 flex-row"><div class="main4 flex-col"></div></div>
          <div class="main5 flex-row"><div class="outer1 flex-col"></div></div>
        </div>
      </div>
      <div class="layer6 flex-col"></div>
      <div class="layer7 flex-col"></div>
      </div>
      <div class="info" v-if="info">
          <div class="mod1 flex-row">
        <img
            @click.stop="info=false"
          class="pic1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbaee696ebb27ebb019468d44c8ac7bcabe494e65c8fab569c6560fcd63f4aec0"
        />
        <img
            
          class="img1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng87335a5924bd056f4135617df7b3f97e0acaaa8692fc0cab1f2ee06a5543c07c"
        />
      </div>
      <div class="mod2 flex-row">
        <div class="outer1 flex-col">
          <div class="box1 flex-col">
            <img
              class="img2"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge29bfd29776017f86fcd86aae81629fe2825373b0baae954cfc80134dc78fd8d"
            />
          </div>
        </div>
      </div>
      <div class="mod3 flex-row" >
        <img
          class="pic2"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2d939b59a8ebf5d5b4189c149fbf2328ce1bc5ec4175498fd3c3ee61c68bae0a"
        />
      </div>
      <div class="mod4 flex-col" ><span class="word1">冒险</span></div>
      <div class="mod5 flex-col" ></div>
      <div class="mod6 flex-col"></div>
      <div class="mod7 flex-col">
        <div class="outer2 flex-col" @click.stop="openCs">
          <div class="group1 flex-row"><div class="main1 flex-col"></div></div>
          <div class="group2 flex-row"><div class="mod8 flex-col"></div></div>
          <div class="group3 flex-row"><div class="group4 flex-col"></div></div>
          <div class="group5 flex-row"><div class="main2 flex-col"></div></div>
        </div>
      </div>
      <div class="mod9 flex-col" ><span class="txt1">自信</span></div>
      <div class="mod10 flex-col" ><span class="info1">后悔</span></div>
      <div class="mod11 flex-col" ></div>
      <div class="mod12 flex-col" ></div>
      <div class="mod13 flex-col" ><span class="info2">冲动</span></div>
      <div class="mod14 flex-col" ><span class="word2">乐观</span></div>
      <div class="mod15 flex-col" ></div>
      <div class="mod16 flex-col" ></div>
      <div class="swiper-container">
          <div class="swiper-wrapper">
              <div class="swiper-slide" v-for="(item,index) in 3" v-bind:key="index">
                <div class="mod17 flex-col" >
                  <div class="layer1 flex-col">
                    <div class="section1 flex-col">
                      <span class="word3">锐意进取策略</span>
                      <span class="info3">中高风险</span>
                    </div>
                    <img
                      class="img3"
                      referrerpolicy="no-referrer"
                      src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2fb8c7e4b11879f3041a861bd87ef4f01e64e99f9262a7e8ca4e7a495090aa19"
                    />
                    <div class="section2 flex-col"></div>
                    <div class="section3 flex-col"></div>
                    <div class="section4 flex-col">
                      <span class="word4">专家会根据行情，结合模型为你调仓</span>
                    </div>
                    <div class="section5 flex-col" @click.stop="openDetail">
                      <span class="word5">立即转入</span>
                    </div>
                    <div class="section6 flex-col">
                      <div class="layer2 flex-col"></div>
                      <span class="info4">根据VCMM®模型测算，投资1万并持有3年</span>
                      <span class="paragraph1">
                        较差情况亏损
                        <br />
                        不超2340.00元
                      </span>
                      <span class="infoBox1">
                        较好情况可
                        <br />
                        赚7240.00元
                      </span>
                    </div>
                  </div>
                  <img
                    class="pic3"
                    referrerpolicy="no-referrer"
                    src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng76b8410215cf5129349da1a8afed9b0614eee7907165a9ca3a786299091abd64"
                  />
                  <img
                    class="img4"
                    referrerpolicy="no-referrer"
                    src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng958842ee19b4b8ca924aebd31bb5189f60c2446185b82f193c4b9ce3fede4a20"
                  />
                  <span class="txt2">+10%</span>
                  <span class="info5">策略说明</span>
                  <span class="word6">35.00%</span>
                  <span class="info6">股票类基金</span>
                  <span class="word7">固收类基金</span>
                  <span class="info7">65.00%</span>
                </div>
              </div> 
            
          </div>
          <!-- 如果需要分页器 -->
          <div class="swiper-pagination"></div> 
          
          <!-- 如果需要导航按钮 -->
          <div class="investproTab investpro-prev swiper-button-prev" id="investpro-prev" @click.stop="prev(1)"></div>
          <div class="investproTab investpro-next swiper-button-next" id="investpro-next" @click.stop="prev(2)"></div>
          
          <!-- 如果需要滚动条 -->
          <!-- <div class="swiper-scrollbar"></div> -->
      </div>
      
      
      <img
        
        class="img5"
        referrerpolicy="no-referrer"
        src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngadd51cd1e695c74a3b56845ecd7df5da068e845996a3c4e2769741d813e05d0b"
      />
      <div class="mod20 flex-col" ></div>
      
      <div class="mod21 flex-col"></div>
      </div>
    </div>
</template>

<script>
import Swiper from 'swiper';
export default {
    data(){
        return{
            info:false,
            swiper:{}
        }
    },
    watch:{
      'info':function(val){
        if(val){
          this.$nextTick(() => {
            this.swiper = new Swiper('.swiper-container',{
              direction: 'horizontal',
              loop: true,
              autoplay: false,
              slidesPerView: "auto",
              centeredSlides:true,
              spaceBetween: 30,
              nextButton: '.swiper-button-next',
              prevButton: '.swiper-button-prev',
              // 如果需要分页器
              pagination: {
                el:'.swiper-pagination',
                clickable:true
              },
              
            })
          })
        }
      }
    },
    created(){

    },
    mounted(){
      
    },
    methods:{
        openUser(){
            this.info = true;
        },
        openCs(){
            this.$router.push({path:'/usercs'})
        },
        openDetail(){
            this.$router.push({path:'/detail'});
        },
         toCard(){
            this.$router.push({path:'/card'})
        },
        prev(type){
          console.log(type)
          if(type == 1){
            this.swiper.slidePrev()
          }else{
            this.swiper.slideNext()
          }
      },
    }
}
</script>

<style lang="scss" scoped>
@important 'swiper/dist/css/swiper.css'
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
}
.no-info{
    .layer1 {
  z-index: auto;
  width: 25.787rem;
  height: 26.08rem;
  margin: 471px 0 0 300px;
}

.layer2 {
  z-index: 4;
  height: 26.08rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngee18f2ac92cfc9be8a93456f2454e4da7ce6c09c49c3dd63ad3266d5f2653009) -59.5px -59.5px
    no-repeat;
    background-size:100% auto;
  width: 25.787rem;
  justify-content: center;
  align-items: center;
}

.bd1 {
  z-index: 6;
  height: 24.587rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngf556742ebc91f23afe5ff29f60f026ca68a99c28918ea38acd98350275cdd2de)
    100% no-repeat;
    background-size:100% auto;
  width: 24.587rem;
}

.img1 {
  z-index: 7;
  width: 24.587rem;
  height: 24.587rem;
}

.layer3 {
  z-index: auto;
  width: 42.374rem;
  height: 15.28rem;
  margin-top: 16rem;
  justify-content: space-between;
}

.img2 {
  z-index: 16;
  width: 8.267rem;
  height: 15.28rem;
}

.section1 {
  z-index: 15;
  width: 24.4rem;
  height: 6.72rem;
  overflow-wrap: break-word;
  text-align: center;
  margin-top: 1.867rem;
  font-size: 0;
}

.word1 {
  font-size: 4.8rem;
  font-family: PingFangSC-Medium;
  color: rgba(0, 0, 0, 1);
  line-height: 6.72rem;
}

.word2 {
  font-size: 4.8rem;
  font-family: PingFangSC-Medium;
  color: rgba(23, 88, 255, 1);
  line-height: 6.72rem;
}

.layer4 {
  z-index: 3;
  position: absolute;
  left: -22.213rem;
  top: 6.454rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
    416.5px -16px no-repeat;
    background-size:100% auto;
}

.layer5 {
  z-index: 8;
  height: 38.4rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngd01581a2abbc882d829f9a1047c04c8360238d9ddc91f5e2c7846c1f0881a547)
    100% no-repeat;
    background-size:100% auto;
  width: 38.4rem;
  justify-content: center;
  align-items: center;
  position: absolute;
  left: 9.6rem;
  top: 18.96rem;
}

.block1 {
  z-index: 9;
  height: 32.747rem;
  border-radius: 50%;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngbb4d17c202d9db1d5c10769cc7f0c07fe3f09103149c91af13307f3819701972)
    100% no-repeat;
    background-size:100% auto;
  width: 32.747rem;
}

.main1 {
  z-index: auto;
  width: 1.147rem;
  height: 1.147rem;
  margin: 425px 0 0 18.5px;
}

.section2 {
  z-index: 13;
  width: 1.147rem;
  height: 1.147rem;
  background-color: rgba(23, 88, 255, 0.74);
  border-radius: 50%;
}

.main2 {
  z-index: auto;
  width: 1.787rem;
  height: 1.787rem;
  margin: -419.5px 0 0 43px;
}

.bd2 {
  z-index: 12;
  width: 1.787rem;
  height: 1.787rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.main3 {
  z-index: auto;
  width: 1.147rem;
  height: 1.147rem;
  margin: 16px 0 0 502.5px;
}

.main4 {
  z-index: 14;
  width: 1.147rem;
  height: 1.147rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.main5 {
  z-index: auto;
  width: 1.787rem;
  height: 1.787rem;
  margin: 374px 0 0 537.5px;
}

.outer1 {
  z-index: 10;
  width: 1.787rem;
  height: 1.787rem;
  background-color: rgba(23, 88, 255, 0.74);
  border-radius: 50%;
}

.layer6 {
  z-index: 11;
  position: absolute;
  left: 27.894rem;
  top: 56.48rem;
  width: 1.787rem;
  height: 1.787rem;
  background-color: rgba(23, 88, 255, 1);
  border-radius: 50%;
}

.layer7 {
  z-index: 2;
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
.info{
  height:100%;
    .mod1 {
    z-index: auto;
    width: 52.72rem;
    height: 3.094rem;
    justify-content: space-between;
    margin: 43.5px 0 0 46px;
  }

  .pic1 {
    z-index: 73;
    width: 1.707rem;
    height: 3.094rem;
  }

  .img1 {
    z-index: 78;
    width: 3.76rem;
    height: 3.094rem;
  }

  .mod2 {
    z-index: auto;
    width: 21.12rem;
    height: 21.36rem;
    margin: 161.5px 0 0 341.5px;
  }

  .outer1 {
    z-index: 6;
    height: 21.36rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge84aeb8c95d4bac6ff11550f0de6d0bb004b6a1716315f14c8a8d6a95d42b161)
      no-repeat;
      background-size:100% auto;
    width: 21.12rem;
    justify-content: center;
    align-items: center;
  }

  .box1 {
    z-index: 8;
    height: 20.134rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2d44a528454dc85bacc8308d8ae8e039477fcf6bae97725d585c8404860a9441)
      100% no-repeat;
      background-size:100% auto;
    width: 20.134rem;
  }

  .img2 {
    z-index: 9;
    width: 20.134rem;
    height: 20.134rem;
  }

  .mod3 {
    z-index: auto;
    width: 8.08rem;
    height: 6.427rem;
    margin: 166.5px 0 0 134.5px;
  }

  .pic2 {
    z-index: 2;
    width: 8.08rem;
    height: 6.427rem;
  }

  .mod4 {
    z-index: 22;
    position: absolute;
    left: 24.48rem;
    top: 3.867rem;
    width: 8.614rem;
    height: 8.614rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngddffaf4102c62d4d4e107f18282ddef22d75d1b3c225b7450ebd2ce3babaa73b)
      100% no-repeat;
      background-size:100% auto;
  }

  .word1 {
    z-index: 26;
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

  .mod5 {
    z-index: 17;
    position: absolute;
    left: 25.307rem;
    top: 4.747rem;
    width: 6.854rem;
    height: 6.854rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
      100% no-repeat;
      background-size:100% auto;
  }

  .mod6 {
    z-index: 4;
    position: absolute;
    left: -22.213rem;
    top: 6.454rem;
    width: 26.987rem;
    height: 27.307rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnge3661f3da031ef3dce933d4071832f4cd9907768ce68a91acf71a115c48fd77a)
      833px -32px no-repeat;
      background-size:100% auto;
  }

  .mod7 {
    z-index: 10;
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
    top: 8.987rem;
  }

  .outer2 {
    z-index: 11;
    height: 26.8rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng42fb6a0cc26de5914328930c01ea8354f44aacc4fb0fb9576f01c10d1941dd0f)
      100% no-repeat;
      background-size:100% auto;
    width: 26.8rem;
  }

  .group1 {
    z-index: auto;
    width: 0.934rem;
    height: 0.934rem;
    margin: 348px 0 0 15px;
  }

  .main1 {
    z-index: 14;
    width: 0.934rem;
    height: 0.934rem;
    background-color: rgba(23, 88, 255, 0.74);
    border-radius: 50%;
  }

  .group2 {
    z-index: auto;
    width: 1.467rem;
    height: 1.467rem;
    margin: -343.5px 0 0 35px;
  }

  .mod8 {
    z-index: 13;
    width: 1.467rem;
    height: 1.467rem;
    background-color: rgba(23, 88, 255, 1);
    border-radius: 50%;
  }

  .group3 {
    z-index: auto;
    width: 0.934rem;
    height: 0.934rem;
    margin: 13px 0 0 425.5px;
  }

  .group4 {
    z-index: 15;
    width: 0.934rem;
    height: 0.934rem;
    background-color: rgba(23, 88, 255, 1);
    border-radius: 50%;
  }

  .group5 {
    z-index: auto;
    width: 1.467rem;
    height: 1.467rem;
    margin: 306.5px 0 0 440px;
  }

  .main2 {
    z-index: 12;
    width: 1.467rem;
    height: 1.467rem;
    background-color: rgba(23, 88, 255, 0.74);
    border-radius: 50%;
  }

  .mod9 {
    z-index: 23;
    position: absolute;
    left: 40.214rem;
    top: 15.68rem;
    width: 8.614rem;
    height: 8.614rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng5eee85a594afe453f38d6639972d5273f1ade261c44e3eacd1fc4e8af3dd4561)
      100% no-repeat;
      background-size:100% auto;
  }

  .txt1 {
    z-index: 27;
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

  .mod10 {
    z-index: 21;
    position: absolute;
    left: 8.774rem;
    top: 15.68rem;
    width: 8.614rem;
    height: 8.614rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng416e7adbfda89ff899fa05d029cbe1c31d09d3a7a72dfb9f4ebf959084b1190d)
      100% no-repeat;
      background-size:100% auto;
  }

  .info1 {
    z-index: 30;
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

  .mod11 {
    z-index: 18;
    position: absolute;
    left: 41.04rem;
    top: 16.56rem;
    width: 6.854rem;
    height: 6.854rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
      100% no-repeat;
      background-size:100% auto;
  }

  .mod12 {
    z-index: 16;
    position: absolute;
    left: 9.6rem;
    top: 16.56rem;
    width: 6.854rem;
    height: 6.854rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
      100% no-repeat;
      background-size:100% auto;
  }

  .mod13 {
    z-index: 24;
    position: absolute;
    left: 35.28rem;
    top: 32.88rem;
    width: 8.614rem;
    height: 8.614rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng713cc98b428511a2e7a688bf0ad1528b7c998095d6e526a1b1ad063470b13a11)
      100% no-repeat;
      background-size:100% auto;
  }

  .info2 {
    z-index: 28;
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

  .mod14 {
    z-index: 25;
    position: absolute;
    left: 14.427rem;
    top: 33.387rem;
    width: 8.614rem;
    height: 8.614rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng4d314e28dbf56b57fbd29c883b46d9412533bfdd5571ccb94fde19c55777f3f1)
      100% no-repeat;
      background-size:100% auto;
  }

  .word2 {
    z-index: 29;
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

  .mod15 {
    z-index: 19;
    position: absolute;
    left: 36.107rem;
    top: 33.76rem;
    width: 6.854rem;
    height: 6.854rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
      100% no-repeat;
      background-size:100% auto;
  }

  .mod16 {
    z-index: 20;
    position: absolute;
    left: 15.254rem;
    top: 34.267rem;
    width: 6.854rem;
    height: 6.854rem;
    border-radius: 50%;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngdaf930cc5a238f8809ed2cc43093384a3de02e6d0915603b8093140465892141)
      100% no-repeat;
      background-size:100% auto;
  }

  .mod17 {
    z-index: 32;
    height: 53.707rem;
    border-radius: 68px;
    background-color: rgba(255, 255, 255, 1);
    box-shadow: 0px 0px 100px 20px rgba(0, 0, 0, 0.06);
    width: 100%;
    justify-content: flex-start;
    position: absolute;
    left: 0;
    top: 0;
  }

  .layer1 {
    z-index: auto;
    width: 33.254rem;
    background:#fff;
    height: 52.694rem;
    margin:0 auto;
  }

  .section1 {
    z-index: 47;
    position: relative;
    width: 37.254rem;
    height: 6.294rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng02ebba1be4e60f7379759c418f4bb60d1b5086e1734d720a75cce3091a023110) -59px -60px
      no-repeat;
      background-size:117% auto;
    align-self: center;
    
  }

  .word3 {
    z-index: 72;
    position: absolute;
    left: 10.534rem;
    top: 0.747rem;
    width: 16.16rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(191, 80, 29, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Semibold;
    line-height: 2.987rem;
    text-align: center;
  }

  .info3 {
    z-index: 55;
    position: absolute;
    left: 15.947rem;
    top: 3.84rem;
    width: 5.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(191, 80, 29, 1);
    font-size: 1.333rem;
    font-family: PingFangSC-Regular;
    line-height: 1.867rem;
    text-align: center;
  }

  .img3 {
    z-index: 56;
    width: 20.107rem;
    height: 14.294rem;
    align-self: center;
    margin-top: 8.32rem;
  }

  .section2 {
    z-index: 85;
    width: 0.774rem;
    height: 0.774rem;
    background-color: rgba(230, 16, 16, 1);
    border-radius: 50%;
    align-self: flex-start;
    margin: 56.5px 0 0 210.5px;
  }

  .section3 {
    z-index: 86;
    width: 0.774rem;
    height: 0.774rem;
    background-color: rgba(23, 88, 255, 1);
    border-radius: 50%;
    align-self: flex-start;
    margin: 21.5px 0 0 210.5px;
  }

  .section4 {
    z-index: 87;
    position: relative;
    width: 22.454rem;
    height: 2.854rem;
    border-radius: 53.5px 53.5px 53.5px 53.5px;
    background-color: rgba(23, 88, 255, 0.21);
    align-self: flex-end;
    margin: 28px 100px 0 0;
  }

  .word4 {
    z-index: 90;
    position: absolute;
    left: 2.694rem;
    top: 0.694rem;
    width: 17.067rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Regular;
    line-height: 1.494rem;
    text-align: center;
  }

  .section5 {
    z-index: 88;
    position: relative;
    width: 34.934rem;
    height: 4.827rem;
    border-radius: 8.5px;
    background-color: rgba(23, 88, 255, 1);
    align-self: center;
    margin-top: 1.174rem;
  }

  .word5 {
    z-index: 91;
    position: absolute;
    left: 9.44rem;
    top: 0.88rem;
    width: 16.16rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(255, 255, 255, 1);
    font-size: 2.133rem;
    font-family: PingFangSC-Medium;
    line-height: 2.987rem;
    text-align: center;
  }

  .section6 {
    z-index: 89;
    height: 6.587rem;
    border-radius: 8.5px;
    background-color: rgba(236, 236, 236, 1);
    align-self: center;
    margin-top: 1.147rem;
    width: 34.934rem;
    justify-content: flex-end;
    padding-bottom: 0.667rem;
    align-items: center;
    position: relative;
  }

  .layer2 {
    z-index: 95;
    width: 0.027rem;
    height: 2.614rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng3fd65a553b6168e79c1b4ddf40c343c4d2dc431219ef520fa4bccbe0ceff0d37)
      100% no-repeat;
      background-size:100% auto;
  }

  .info4 {
    z-index: 92;
    position: absolute;
    left: 7.36rem;
    top: 0.774rem;
    width: 20.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(147, 147, 147, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Regular;
    line-height: 1.494rem;
    text-align: center;
  }

  .paragraph1 {
    z-index: 94;
    position: absolute;
    left: 19.387rem;
    top: 2.907rem;
    width: 7.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(147, 147, 147, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Regular;
    line-height: 1.494rem;
    text-align: left;
  }

  .infoBox1 {
    z-index: 93;
    position: absolute;
    left: 9.334rem;
    top: 2.907rem;
    width: 6.214rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(147, 147, 147, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Regular;
    line-height: 1.494rem;
    text-align: right;
  }

  .pic3 {
    z-index: 61;
    position: absolute;
    left: 18.64rem;
    top: 8.774rem;
    width: 10.08rem;
    height: 11.094rem;
  }

  .img4 {
    z-index: 66;
    position: absolute;
    left: 9.414rem;
    top: 8.774rem;
    width: 9.254rem;
    height: 7.494rem;
  }

  .txt2 {
    z-index: 71;
    position: absolute;
    left: 13.6rem;
    top: 15.014rem;
    width: 10.08rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 3.2rem;
    font-family: PingFangSC-Semibold;
    line-height: 4.48rem;
    text-align: center;
  }

  .info5 {
    z-index: 50;
    position: absolute;
    left: 15.974rem;
    top: 20.827rem;
    width: 5.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(143, 143, 143, 1);
    font-size: 1.333rem;
    font-family: PingFangSC-Regular;
    line-height: 1.867rem;
    text-align: center;
  }

  .word6 {
    z-index: 52;
    position: absolute;
    left: 21.307rem;
    top: 31.574rem;
    width: 3.92rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(230, 16, 16, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Medium;
    line-height: 1.494rem;
    text-align: center;
  }

  .info6 {
    z-index: 51;
    position: absolute;
    left: 14.347rem;
    top: 31.574rem;
    width: 5.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Regular;
    line-height: 1.494rem;
    text-align: center;
  }

  .word7 {
    z-index: 54;
    position: absolute;
    left: 14.347rem;
    top: 33.467rem;
    width: 5.334rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(0, 0, 0, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Regular;
    line-height: 1.494rem;
    text-align: center;
  }

  .info7 {
    z-index: 53;
    position: absolute;
    left: 21.307rem;
    top: 33.467rem;
    width: 3.92rem;
    display: block;
    overflow-wrap: break-word;
    color: rgba(23, 88, 255, 1);
    font-size: 1.066rem;
    font-family: PingFangSC-Medium;
    line-height: 1.494rem;
    text-align: center;
  }

  .mod18 {
    z-index: 40;
    position: absolute;
    left: -27.466rem;
    top: 49.574rem;
    width: 34.027rem;
    height: 49.04rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng13b1c79a7d96fc8d86620d077b75e2bcc0de759df6860a9454dbd70faaf4c238) -127px -65px
      no-repeat;
      background-size:134% auto;
  }

  .mod19 {
    z-index: 33;
    position: absolute;
    left: 51.147rem;
    top: 49.574rem;
    width: 34.027rem;
    height: 49.04rem;
    background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng84ca34a7e5dfc949d63324681dda0191ed30562ee47f0ddcf4796e81f0da7656) -95px -147px
      no-repeat;
      background-size:140% auto;
  }

  .img5 {
    z-index: 31;
    position: absolute;
    left: 0;
    top: 53.174rem;
    width: 57.6rem;
    height: 49.227rem;
  }

  .mod20 {
    z-index: 1;
    position: absolute;
    left: 25.254rem;
    top: 67.2rem;
    width: 7.147rem;
    height: 2.214rem;
    border-radius: 20.75px 20.75px 20.75px 20.75px;
    border: 2px solid rgba(151, 151, 151, 1);
  }

  .pic4 {
    z-index: 75;
    position: absolute;
    left: 2.614rem;
    top: 68.8rem;
    width: 52.4rem;
    height: 3.094rem;
  }

  .mod21 {
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

  .swiper-container {
      width: 100%;
      height:53.707rem;
      margin-bottom:1rem;
      overflow: visible!important;
      z-index:65;
      position:absolute;
      bottom:20px;
  }
  .swiper-container .swiper-wrapper .swiper-slide{position:relative; width: 37.254rem; border-radius: 20px;}
  .swiper-container .swiper-wrapper .swiper-slide-prev{ transform:scale(0.8)}
  .swiper-container .swiper-wrapper .swiper-slide-next{ transform:scale(0.8)}
  .swiper-container .swiper-wrapper .swiper-slide-active{ width: 37.254rem;}

  .swiper-pagination{
      bottom: -30px!important;
  }
  .swiper-pagination .swiper-pagination-bullet{width: 12px; height: 12px; background: #ff1e1e;}
  .swiper-pagination .swiper-pagination-bullet-active{width: 21px; height: 12px; background: #e75230; border-radius: 6px;}
  .investproTab{width:5rem;height:5rem;border-radius:50%;z-index:65;background:url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngef15d6cc049821127d03c200bc43e161f7cf26da2b6092b5255376aaf57f8886) left center no-repeat;background:auto 5rem;position:absolute;left:0;top:20.6rem;left:6rem;}
  .investpro-next{right:6rem;left:auto;background:url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngef15d6cc049821127d03c200bc43e161f7cf26da2b6092b5255376aaf57f8886) right center}


}



</style>