<template>
  <div class="page flex-col">
      <!-- <div class="section1 flex-col">
        <img
          class="pic1"
          referrerpolicy="no-referrer"
          src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngba7ee175c4a17203d134d8066bfaeb2eab9a147796871dc6f009c2d4af9892ca"
        />
      </div> -->
      <div class="section2 flex-col"></div>
      <div class="section3">
        <span class="word1">恭喜你完成了测试，打败了全国</span>
        <span class="word2">79%</span>
        <span class="txt1">的用户！</span>
      </div>
      <div class="section4 flex-col">
        <div class="section5 flex-col">
          <div class="bd1 flex-col">
            <img
              class="pic2"
              referrerpolicy="no-referrer"
              src="https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng0f07d8516a7b9290b167884efa5418bd06f53b59ce12cc888dc41e3027d9859f"
            />
          </div>
          <div class="bd2 flex-col">
            <span class="word3" @click.stop="viewText">查看理财性格</span>
          </div>
        </div>
        <span class="word4">+10.00%</span>
        <span class="txt2">11000.00</span>
        <span class="word5">最终总资产</span>
        <span class="info1">收益率</span>
        <span class="info2">159****9170</span>
        <span class="info3">Li</span>
      </div>
      <div class="section6 flex-col"></div>
    </div>
</template>

<script>
export default {
    data(){
        return{

        }
    },
    methods:{
        viewText(){
            this.$router.push({path:'/viewtext'});
        }
    }
}
</script>

<style lang="scss" scoped>
    html {
  font-size:18.75px;
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

// .section1 {
//   z-index: 18;
//   height: 9.414rem;
//   background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPngd87c89ac3cabfa0284fcd7d1c6a9b32de683c3db1cf40ea1314d218d8d77f401) 0px -45px
//     no-repeat;
//     background-size:100% auto;
//   width: 38.427rem;
//   justify-content: center;
//   align-items: center;
// }

.pic1 {
  z-index: 30;
  width: 4.187rem;
  height: 4.187rem;
}

.section2 {
  z-index: 3;
  position: absolute;
  left: -22.826rem;
  top: 34.214rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPnga890d1a60155ace076854425fe3b325df2ef2f3f948825cf0eac19d8cd30a4d9)
    856px -19px no-repeat;
    background-size:100% auto;
}

.section3 {
  z-index: 11;
  position: absolute;
  left: 0.774rem;
  top: 69.307rem;
  width: 56.054rem;
  height: 4.48rem;
  overflow-wrap: break-word;
  text-align: center;
  font-size: 0;
}

.word1 {
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  color: rgba(109, 114, 120, 1);
  line-height: 2.987rem;
}

.word2 {
  font-size: 3.2rem;
  font-family: PingFangSC-Medium;
  color: rgba(23, 88, 255, 1);
  line-height: 2.987rem;
}

.txt1 {
  font-size: 2.133rem;
  font-family: PingFangSC-Medium;
  color: rgba(109, 114, 120, 1);
  line-height: 2.987rem;
}

.section4 {
  z-index: 4;
  height: 86.774rem;
  border-radius: 114px;
  background-color: rgba(255, 255, 255, 1);
  box-shadow: 0px 0px 100px 20px rgba(0, 0, 0, 0.06);
  width: 53.334rem;
  justify-content: flex-start;
  align-items: flex-start;
  position: absolute;
  left: 2.134rem;
  top: 1.6rem;
  padding: 60.5px 0 0 73.5px;
}

.section5 {
  z-index: auto;
  width: 35.574rem;
  height: 79.2rem;
}

.bd1 {
  z-index: 14;
  position: relative;
  width: 16.72rem;
  height: 16.72rem;
  border-radius:36px;
  overflow: hidden;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng5544ccb760e81cf554a979e793ef39585c11a7c0f15f9664ed1609a12d4db583)
    100% no-repeat;
    background-size:100% auto;
  align-self: flex-start;
}

.pic2 {
  z-index: 15;
  position: absolute;
  left: 0;
  top: 0;
  width: 16.72rem;
  height: 16.72rem;
}

.bd2 {
  z-index: 16;
  position: relative;
  width: 25.654rem;
  height: 6.694rem;
  border-radius: 62.75px 62.75px 62.75px 62.75px;
  background-color: rgba(23, 88, 255, 1);
  align-self: flex-end;
  margin-top: 55.787rem;
}

.word3 {
  z-index: 17;
  position: absolute;
  left: 3.894rem;
  top: 1.467rem;
  width: 17.894rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(255, 255, 255, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: center;
}

.word4 {
  z-index: 8;
  position: absolute;
  left: 3.92rem;
  top: 53.76rem;
  width: 18.747rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 4.266rem;
  font-family: PingFangSC-Medium;
  line-height: 5.974rem;
  text-align: left;
}

.txt2 {
  z-index: 7;
  position: absolute;
  left: 3.92rem;
  top: 35.307rem;
  width: 18.747rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(23, 88, 255, 1);
  font-size: 4.266rem;
  font-family: PingFangSC-Medium;
  line-height: 5.974rem;
  text-align: left;
}

.word5 {
  z-index: 5;
  position: absolute;
  left: 3.92rem;
  top: 30.374rem;
  width: 18.747rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.info1 {
  z-index: 6;
  position: absolute;
  left: 4.08rem;
  top: 48.827rem;
  width: 11.254rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.info2 {
  z-index: 10;
  position: absolute;
  left: 25.307rem;
  top: 13.387rem;
  width: 16.72rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(109, 114, 120, 1);
  font-size: 2.666rem;
  font-family: PingFangSC-Medium;
  line-height: 3.734rem;
  text-align: left;
}

.info3 {
  z-index: 9;
  position: absolute;
  left: 25.307rem;
  top: 8.187rem;
  width: 13.12rem;
  display: block;
  overflow-wrap: break-word;
  color: rgba(0, 0, 0, 1);
  font-size: 3.2rem;
  font-family: PingFangSC-Medium;
  line-height: 4.48rem;
  text-align: left;
}

.section6 {
  z-index: 2;
  position: absolute;
  left: 51.467rem;
  top: 68.027rem;
  width: 26.987rem;
  height: 27.307rem;
  background: url(https://lanhu.oss-cn-beijing.aliyuncs.com/SketchPng2576e4a9e101c98b49f05ddaf263229cec676dafd8b8244a131052f55b22854e) -119px -60px
    no-repeat;
    background-size:100% auto;
}

</style>