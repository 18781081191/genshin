<template>
  <div class="weaperBox">
    <div class="tabBox">
      <div
        class="box1"
        :class="{ active: currentTab == 'A' }"
        @click="toggletab('A')"
      >
        <img src="../assets/images/Icon_Artifacts.png" alt="" />
      </div>
      <div
        class="box1"
        :class="{ active: currentTab == 'B' }"
        @click="toggletab('B')"
      >
        <img src="../assets/images/Icon_Plume.png" alt="" />
      </div>
      <div
        class="box1"
        :class="{ active: currentTab == 'C' }"
        @click="toggletab('C')"
      >
        <img src="../assets/images/Icon_Flower.png" alt="" />
      </div>
      <div
        class="box1"
        :class="{ active: currentTab == 'D' }"
        @click="toggletab('D')"
      >
        <img src="../assets/images/Icon_Sands.png" alt="" />
      </div>
      <div
        class="box1"
        :class="{ active: currentTab == 'E' }"
        @click="toggletab('E')"
      >
        <img src="../assets/images/Icon_Circlet.png" alt="" />
      </div>
      <div
        class="box1"
        :class="{ active: currentTab == 'F' }"
        @click="toggletab('F')"
      >
        <img src="../assets/images/Icon_Goblet.png" alt="" />
      </div>
    </div>
    <div class="left">
      <div class="box2">
        <div class="inside">
          <div class="in">死之羽</div>
          <div class="in">
            <i class="fa fa-star"></i>
            <i class="fa fa-star"></i>
            <i class="fa fa-star"></i>
            <i class="fa fa-star"></i>
            <i class="fa fa-star"></i>
          </div>
          <div class="in">攻击力</div>
          <div class="in">47</div>
          <img
            src="../assets/images/Artifacts/ArchaicPetra/Circlet.png"
            alt=""
          />
          <span>+20</span>
        </div>
      </div>
      <div class="right">
        <div class="datailBox">
          <div class="top">
            <div class="bian">
              <img src="../assets/images/artifact_arrow.png" alt="" />
              <img src="../assets/images/artifact_arrow.png" alt="" />
              <span>&nbsp;&nbsp;&nbsp;梦醒之瓢</span>
            </div>
          </div>
          <div class="nameBox">
            <span>空之杯</span>
            <span>攻击杯</span>
            <span>7.0%</span>
            <div class="in st">
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
              <i class="fa fa-star"></i>
            </div>
            <img
              src="../assets/images/Artifacts/ArchaicPetra/Circlet.png"
              alt=""
            />
          </div>
          <div class="wbottom">
            <div class="bo">
              <span>+20</span>
              <div class="bor">
                <svg
                  t="1676894905172"
                  class="icon"
                  viewBox="0 0 1024 1024"
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  p-id="12738"
                  width="20"
                  height="20"
                >
                  <path
                    d="M832 464H332V240c0-30.9 25.1-56 56-56h248c30.9 0 56 25.1 56 56v68c0 4.4 3.6 8 8 8h56c4.4 0 8-3.6 8-8v-68c0-70.7-57.3-128-128-128H388c-70.7 0-128 57.3-128 128v224h-68c-17.7 0-32 14.3-32 32v384c0 17.7 14.3 32 32 32h640c17.7 0 32-14.3 32-32V496c0-17.7-14.3-32-32-32zM540 701v53c0 4.4-3.6 8-8 8h-40c-4.4 0-8-3.6-8-8v-53c-12.1-8.7-20-22.9-20-39 0-26.5 21.5-48 48-48s48 21.5 48 48c0 16.1-7.9 30.3-20 39z"
                    p-id="12739"
                    fill="#bfbfbf"
                  ></path>
                </svg>
              </div>
            </div>
            <div class="nbox">
              <span>·&nbsp;防御力+5.1%</span>
              <span>·&nbsp;防御力+5.1%</span>
              <span>·&nbsp;防御力+5.1%</span>
              <span>·&nbsp;防御力+5.1%</span>
            </div>
            <div class="na">追忆之注连:</div>
            <div class="word">
              <span><i class="fa fa-ban"></i>2件套: 攻击力提高18%。</span>
              <span
                ><i class="fa fa-ban"></i>4件套:
                施放元素战技时，如果角色的元素能量高于或等于15点，则会流失15点元素能量，使接下来的10秒内，普通攻击、重击、下落攻击造成的伤害提高50%，持续期间内该效果不会再次触发。</span
              >
            </div>
          </div>
        </div>
        <div class="btnBox1">
          <div class="btn">
            <span class="squareinbox1"></span>
            装备
          </div>
          <div class="btn" squareinbox1>
            <span class="squareinbox2"></span>
            强化界面
          </div>
        </div>
        <div class="strongBox">
          <div class="box">◆&nbsp;通用操作</div>
          <div class="btnBox">
            <div class="btn">强化</div>
            <div class="btn">重置</div>
            <div class="btn">删除</div>
          </div>
          <div class="box">◆&nbsp;精准强化</div>
          <div class="box precise_strong">
            <div class="precise_strong_box">
              <span style="color: #93806a">•&nbsp;元素充能效率+6.5%</span
              >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<button>
                强化
              </button>
            </div>
            <div class="box">◆&nbsp;强化幅度</div>
          </div>
          <div class="seclectBox">
            <select id="select">
              <option value="随机">随机</option>
              <option value="最低">最低</option>
              <option value="较低">较低</option>
              <option value="较高">较高</option>
              <option value="最高">最高</option>
            </select>
          </div>
        </div>
        <div class="scoreBox">
          <div class="scoreBox_center">
            <div class="top">
              副词条评分（beta）: &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
              <span>99.99</span>
            </div>
            <div class="scoreBottom">
              <div class="score">
                <span>攻击力</span>
                <span>99%</span>
                <div class="bar">
                  <div class="bar_s"></div>
                </div>
              </div>
              <div class="score">
                <span>攻击力</span>
                <span>99%</span>
                <div class="bar">
                  <div class="bar_s"></div>
                </div>
              </div>
              <div class="score">
                <span>攻击力</span>
                <span>99%</span>
                <div class="bar">
                  <div class="bar_s"></div>
                </div>
              </div>
              <div class="score">
                <span>攻击力</span>
                <span>99%</span>
                <div class="bar">
                  <div class="bar_s"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <button class="score_standard">评分标准</button>
      </div>
    </div>
  </div>
</template>
    
 <script>
export default {
  created() {
    // this.store();
  },
  data() {
    return {
      currentTab: "A",
    };
  },
  methods: {
    // store() {
    //   let Relics = [];
    //   localStorage.setItem("Relics", Relics);
    // },
    toggletab(val) {
      this.currentTab = val;
    },
  },
};
</script>
    
    <style lang="scss" scoped>
@import "../../node_modules/font-awesome/css/font-awesome.min.css";
.weaperBox {
  width: 80rem;
  height: 100%;
  overflow: hidden;
  margin: 0 auto;
  position: relative;
  .tabBox {
    width: 60rem;
    height: 8%;
    background-color: #cbc4b6;
    display: flex;
    justify-content: space-around;
    align-items: center;
    .box1 {
      width: 8rem;
      height: 2.4rem;
      border-radius: 0.48rem;
      background-color: #dad6cc;
      display: flex;
      justify-content: center;
      align-items: center;
      opacity: 0.4;
      > img {
        width: 2rem;
        height: 2rem;
      }
    }
  }
  .left {
    width: 60rem;
    height: 92%;
    background-color: #c3bbab;
    overflow: hidden;
    padding-top: 0.6rem;
    padding-left: 2.2rem;
    padding-right: 2.2rem;
    box-sizing: border-box;
    overflow-y: scroll;
    overflow-x: hidden;
    .box2 {
      width: 10.2rem;
      height: 6rem;
      background-color: #ece5d8;
      border-radius: 0.38rem 0.38rem;

      .inside {
        width: 100%;
        height: 100%;
        border-radius: 0.38rem 0.38rem 1.8rem;
        background-color: rgb(207, 122, 38);
        padding-left: 0.6rem;
        padding-right: 0.6rem;
        padding-top: 0.6rem;
        padding-bottom: 0.6rem;
        box-sizing: border-box;
        position: relative;
        overflow: hidden;
        > img {
          width: 6rem;
          height: 6rem;
          position: absolute;
          right: 0.88rem;
          top: 0;
        }
        > span {
          display: block;
          text-align: center;
          line-height: 0.2rem;
          position: absolute;
          right: 0.8rem;
          top: 4rem;
          background-color: #39444f;
          padding: 0.4rem 0.2rem 0.4rem;
          color: white;
          border-radius: 0.04rem;
          font-size: 0.8rem;
        }
        .in {
          font-size: 0.28rem;
          color: white;
          font-weight: 600;
          margin-top: 0.16rem;
        }
        .in:nth-of-type(3) {
          color: #ddb6a5 !important;
        }
      }
    }
  }
  .right {
    width: 20rem;
    height: 86vh;
    position: absolute;
    right: 0;
    padding-top: 0.2rem;
    background-color: #c3bbab;
    top: 0;
    overflow-y: scroll;
    padding: 9.75px;
    box-sizing: border-box;
    &::-webkit-scrollbar {
      display: none;
    }
    .datailBox {
      width: 18rem;
      margin: 0 auto;
      .top {
        width: 100%;
        height: 1.8rem;
        background-color: #bc6832;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        .bian {
          width: 18.7rem;
          height: 1.6rem;
          border: 0.01rem solid rgba(144, 82, 41, 0.7);
          > img:nth-of-type(1) {
            width: 0.6rem;
            height: 0.6rem;
            position: absolute;
            left: 0rem;
            top: 0.6rem;
          }
          > img:nth-of-type(2) {
            width: 0.6rem;
            height: 0.6rem;
            transform: rotate(180deg);
            position: absolute;
            right: 0px;
            top: 0.6rem;
          }
          > span {
            color: white;
            font-weight: 600;
          }
        }
      }
      > .nameBox {
        width: 100%;
        height: 8rem;
        padding: 0.1rem 0.3rem 0.24rem 0.8rem;
        box-sizing: border-box;
        overflow: hidden;
        background-image: linear-gradient(
            to bottom right,
            rgba(110, 72, 72, 0.5) 15%,
            rgba(225, 125, 40, 0.5),
            rgba(255, 175, 45, 0.7) 95%
          ),
          url(../assets/images/item_bg.png);
        position: relative;
        border-bottom: 0.3rem solid rgb(0, 0, 0, 0.2);
        box-sizing: border-box;
        span:nth-of-type(1) {
          color: white;
          font-size: 0.24rem;
          font-weight: 560;
        }
        span:nth-of-type(2) {
          color: #ddb6a5 !important;
          font-size: 0.24rem;
          font-weight: 560;
          display: block;
          margin-top: 1.6rem;
        }
        span:nth-of-type(3) {
          color: white;
          font-size: 1.3rem;
          font-weight: 560;
          display: block;
        }
        .st {
          width: 5rem;
          display: flex;
          justify-content: space-between;
          margin-top: 0.6rem;
        }
        > img {
          position: absolute;
          width: 8rem;
          height: 8rem;
          right: 1rem;
          top: 0px;
        }
      }
      > .wbottom {
        width: 100%;
        height: 19.8rem;
        padding-top: 0.8rem;
        padding-bottom: 0.53rem;
        padding-left: 0.8rem;
        padding-right: 1.8rem;
        background-color: #ece5d8;
        box-sizing: border-box;
        > .bo {
          width: 100%;
          display: flex;
          justify-content: space-between;
          > span {
            width: 2rem;
            display: block;
            text-align: center;
            line-height: 0.13rem;
            background-color: #39444f;
            padding: 0.4rem 0.08rem 0.4rem;
            color: white;
            border-radius: 0.28rem;
            font-size: 0.16rem;
          }
          .bor {
            width: 24px;
            height: 24px;
            display: flex;
            justify-content: center;
            align-items: center;
            border: 1px solid #bfbfbf;
            border-radius: 4px;
          }
        }
        .nbox {
          margin-top: 0.8rem;
          > span {
            display: block;
            margin-top: 0.2rem;
            color: #4c5668;
            font-size: 0.8rem;
            font-weight: 700;
          }
        }
        .na {
          color: #5cb256;
          font-size: 0.8rem;
          font-weight: 700;
          margin-top: 0.3rem;
          margin-bottom: 0.3rem;
          margin-left: -0.28rem;
        }
        .word {
          span {
            display: block;
            font-size: 0.8rem;
            position: relative;
            left: 0.3rem;
            font-weight: 700;
            color: #717782;
            > i {
              color: #717782;
              position: absolute;
              left: -0.7rem;
              top: 0.16rem;
              opacity: 0.5;
            }
          }
        }
      }
    }
    .btnBox1 {
      width: 18rem;
      margin: 0.6rem auto;
      display: flex;
      justify-content: space-between;
      > .btn {
        width: 45%;
        text-align: center;
        background-color: #ece5d8;
        padding-top: 0.6rem;
        padding-bottom: 0.6rem;
        border-radius: 1.5625rem;
        font-weight: 800;
        cursor: pointer;
        .squareinbox1 {
          position: relative;
          float: left;
          margin-top: 0.1rem;
          margin-left: 0.6rem;
          height: 1.2rem;
          width: 1.2rem;
          background-color: #303030;
          border-radius: 0.125rem;
          &::after {
            content: "";
            position: absolute;
            inset: 0.25rem;
            border: 0.125rem solid #f5c332;
          }
        }
        .squareinbox2 {
          position: relative;
          float: left;
          margin-left: 0.6rem;
          height: 1.4rem;
          width: 1.4rem;
          border-radius: 100rem;
          background-color: #303030;
          &::after {
            content: "";
            position: absolute;
            inset: 0.25rem;
            border: 0.125rem solid #f5c332;
            border-radius: 100rem;
          }
        }
      }
    }
    .strongBox {
      width: 18rem;
      margin: 1.2rem auto;
      background-color: #dfd5c0;
      padding: 0.5rem;
      box-sizing: border-box;
      > .box {
        width: 100%;
        border-bottom: 0.18rem solid #d1c0af;
        padding-top: 0.1rem;
        padding-bottom: 0.1rem;
        font-size: 0.9375rem;
        color: #a55843;
        font-weight: 700;
      }
      > .btnBox {
        width: 100%;
        display: flex;
        justify-content: space-between;
        margin-top: 0.5rem;
        margin-bottom: 0.5rem;

        > .btn {
          width: 3.8rem;
          background-color: #ece5d8;
          border-radius: 1.5625rem;
          padding: 0.1rem;
          text-align: center;
          font-weight: 700;
          cursor: pointer;
        }
      }
      .precise_strong {
        width: 100%;
        padding-top: 0.3rem;
        padding-bottom: 0.6rem;
        overflow: hidden;
        .precise_strong_box {
          margin-bottom: 1.2rem;
          > button {
            border: none;
            outline: none;
            width: 3.9rem;
            background-color: #ece5d8 !important;
            border-radius: 1.5625rem !important;
            font-weight: 700;
          }
        }
      }
      .seclectBox {
        box-sizing: border-box;
        width: 100%;
        height: 2.4rem;
        background-color: #ffffff;
        margin-top: 0.6rem;
        border-radius: 0.2rem;
        padding: 0.4rem;
        > select {
          border: none;
          outline: none;
          width: 100%;
          height: 100%;
          font-weight: 700;
          option {
            font-weight: 700;
          }
        }
      }
    }
    .scoreBox {
      width: 18rem;
      margin: 1.2rem auto;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #f9f6f2;
      height: 11rem;
      .scoreBox_center {
        width: 96%;
        border: 0.01rem solid gainsboro;
        height: 96%;
        padding-top: 0.1rem;
        padding-bottom: 0.1rem;
        padding-left: 0.6rem;
        padding-right: 0.6rem;
        box-sizing: border-box;
        > .top {
          border-bottom: 0.1rem solid #adabaa;
          font-weight: 700;
          height: 1.8rem;
          > span {
            font-weight: 700;
          }
        }
        > .scoreBottom {
          width: 100%;
          .score {
            width: 100%;
            height: 2rem;
            display: flex;
            justify-content: space-between;
            align-content: space-around;
            flex-wrap: wrap;
            > span:nth-of-type(1) {
              font-weight: 700;
            }
            > span:nth-of-type(2) {
              font-weight: 700;
              color: #d3bc8e;
            }
            .bar {
              width: 100%;
              height: 0.4rem;
              background-color: #4c5668;
              border-radius: 0.2rem;
              .bar_s {
                width: 63%;
                height: 0.4rem;
                background-color: #d3bc8e;
                border-radius: 0.2rem;
              }
            }
          }
        }
      }
    }
    .score_standard {
      outline: none;
      display: block;
      margin-top: 0.5rem;
      margin-bottom: 0.5rem;
      position: relative;
      color: #ece5d8 !important;
      background-color: #495366 !important;
      border-radius: 1.5625rem !important;
      font-weight: 700;
      margin-left: 0.6rem;
      padding: 0.25rem 0.5rem;
      font-size: 0.875rem;
      border: 0.16rem solid transparent;
      box-sizing: border-box;
      &:hover {
        border: 0.16rem solid #ffe6b2;
      }
    }
  }
}
.active {
  background-color: white !important;
  opacity: 1 !important;
}
.fa-star {
  color: #ffcc32;
}
</style>