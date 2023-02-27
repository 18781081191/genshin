<template>
  <div id="home">
    <div id="header">
      <div class="center">
        <div class="left">
          <span>圣遗物强化模拟器</span>
        </div>
        <div class="right">
          <span>圣遗物&nbsp;1/2000</span>
        </div>
      </div>
    </div>
    <img src="../assets/images/genshin-symbol.png" alt="" />
    <div class="containter"> 
      <Weaper></Weaper>
    </div>
    <div class="bottom"></div>
  </div>
</template>

<script>
import Weaper from "../components/weaper.vue";
export default {
  components: {
    Weaper
  },
  methods: {},
}

</script>
<style lang="scss">
#home{
  width: 100%;
  position: relative;
  background-color: #b4aa96;
  height: 100vh;
  #header{
    width: 100%;
    height: 6vh;
    background-color: rgba(0, 0, 0, 0.5);
    padding-top: 0.11rem;
    padding-bottom: 0.11rem;
    position: relative;
    .center{
      height: 100%;
      margin: 0 auto;
      padding-left: 2.8rem;
      display: flex;
      align-items: center;
      box-sizing: border-box;
      .left{
        width: 8.2rem;
        border-left: 0.20rem solid #fd7e14;
        border-bottom: 0.01rem solid #fd7e14;
        margin-left: 0.53rem;
        box-sizing: border-box;
        >span {
          color: #ece5d8;
          font-weight: 750;
          font-size: 1rem;
        }
      }
      .right {
        position: absolute;
        right: 0.8rem;
        >span {
          color: #d3bc8e;
          font-weight: 750;
        }
      }
    }
  }
  .containter {
    width: 100%;
    height: 86vh;
  }
  .bottom {
    width: 100%;
    height: 8vh;
    padding-top: 0.17rem;
    padding-bottom: 0.17rem;
    padding-left: 0.67rem;
    padding-right: 0.67rem;
    box-sizing: border-box;
    overflow: hidden;
    background-color: #d2cab0;
    position: fixed;
    bottom: 0;
  }
  > img {
    position: absolute;
    z-index: 0;
    height: 60vh;
    top: -27vh;
    left: -23vh;
    opacity: 0.2;
  }
}
</style>