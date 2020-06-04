<template>
  <div class="home">
    <div class="banner">
      <div class="ban-box">
        <span class="dots">
          <span class="dot-box" v-for="index in 5" :key="index">
            <td class="dot"></td>
          </span>
        </span>
        <div class="ban-img">
          <span class="l-arrow">《</span>
          <span class="r-arrow">》</span>

          <img
            width="100%"
            src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/7e882fcbdcafc352dde03c741836399b.jpg?thumb=1&amp;w=1839&amp;h=690&amp;f=webp&amp;q=90"
          />
        </div>
        <div class="ban-list">
          <li v-for="(item,index) in list" :key="index">
            <span class="list-item">
              {{item.text}}
              <span class="fr more">></span>
            </span>
          </li>
        </div>
      </div>
      <div class="ad-box">
        <div class="func-btn">
          <tr v-for="index in 2" :key="index">
            <td class="func-td" v-for="index in 3" :key="index">
              <div class="btn" :class="index== 1||2||3?' bot-line':''">
                <img src="@/assets/icon/coin.png" alt />
                <p>小米秒杀</p>
                <div class="block-tl"></div>
                <div class="block-tr"></div>
                <div class="block-bl"></div>
                <div class="block-br"></div>
              </div>
            </td>
          </tr>
        </div>
        <div class="img-box">
          <img
            class="func-img"
            src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/35a2239e10e392af73b6b7a737a039d6.jpg?w=632&amp;h=340"
            alt
          />
          <img
            class="func-img"
            src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/fbff319c7dd00e75c9758acf248d3784.jpg?w=632&amp;h=340"
            alt
          />
          <img
            class="func-img"
            src="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/816a66edef10673b4768128b41804cae.jpg?w=632&amp;h=340"
            alt
          />
        </div>
      </div>
    </div>
    <div class="shop-cards">
      <div class="shangou">
        <div class="gou-text">小米闪购</div>
        <div class="arrow-box">
          <span class="arrow">《</span>
          <span class="arrow arrow-r">》</span>
        </div>
      </div>
      <div class="card-box">
        <div class="card">
          <div class="changci">10:00场</div>
          <div class="flash">
            <img
              src="data:img/jpg;base64,iVBORw0KGgoAAAANSUhEUgAAACIAAAA1CAYAAAAklDnhAAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJ
               WFnZVJlYWR5ccllPAAAAyNpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdp
               j0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6
               D0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNS1jMDE0IDc5LjE1
               TQ4MSwgMjAxMy8wMy8xMy0xMjowOToxNSAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJo
               HRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlw
               GlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAv
               iB4bWxuczp4bXBNTT0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL21tLyIgeG1sbnM6c3RS
               WY9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZVJlZiMiIHhtcDpD
               mVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIChNYWNpbnRvc2gpIiB4bXBNTTpJbnN0YW5j
               UlEPSJ4bXAuaWlkOjY4Q0ZFMkY5MTJFNzExRThCMkM4OEM1RTNBNjczQUVBIiB4bXBNTTpEb2N1
               WVudElEPSJ4bXAuZGlkOjY4Q0ZFMkZBMTJFNzExRThCMkM4OEM1RTNBNjczQUVBIj4gPHhtcE1N
               kRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6NjhDRkUyRjcxMkU3MTFFOEIy
               zg4QzVFM0E2NzNBRUEiIHN0UmVmOmRvY3VtZW50SUQ9InhtcC5kaWQ6NjhDRkUyRjgxMkU3MTFF
               EIyQzg4QzVFM0E2NzNBRUEiLz4gPC9yZGY6RGVzY3JpcHRpb24+IDwvcmRmOlJERj4gPC94Onht
               G1ldGE+IDw/eHBhY2tldCBlbmQ9InIiPz5oEyacAAACoklEQVR42sSYv0tbURTHX0LqD6T4g4pE
               HDoUOloBxVd/QFFEcQqWtrSKlKFmmAslopohzgIbv4FwUEE0clFujiIi+BSIbRQ0ooKRReRULHf
               48Qgu++c3/FAx+iyU3eJzf3nnPuC/1qavQ04zVY8szjCHRGNN9cBD6DSkOJKzAGzsOaH/AW1FuY
               Rg4EH/oiJSCTxYk1sDK7T86Iu9BraHED/Au9wlVkYdg2lAiC/rBhYnIB/DIUOQj2M9/UkWkCsQN
               bbA8l0vqIhMgXIDiZ/gFbgxEakBEwYSf8Eg+OM3gCsyA8oMRETy25UN4IjUgVEDiW2wGDSIIzIL
               jUljsFLv3WhIvKYFphOXNO6OOUMDhKZA7qFcQF85Q6WXeQpeKEpcULlvY8xthp8iwR8I93qLLb7
               nOsSPWNfhd6Bro99yHqTi9IhyWzEXIsIXbSG7Djt1jbQHsBZkMkyZRs13wpgIRoiJKy7dsBWh1L
               N5Vt3JFQrQ2XMYeGKBk5yvSI7aRQ4k0eA4uZZlVPM47lDgTZxd6lKb4AcqkLuKSZiIdVGsiVFNc
               DV9yT1Orekjoe+MDw4pHqwmaJewit66Ql0QaX+DOTaZe4DitAFZxQaaEynKnJ6KCDeaQAtj3A7V
               BtXIpwT3iFV06zqquaKPKEtKIsM6Mo/StoWiQeMvSCJjO4+54hEwTCjuTk0STgckUm6QxTY3LgU
               c+/jyFrblyKCIkKbnPjSkT8HDGV5saVyBAtVHZz40Ik7HNTRtrcuBARF2tQbW5ciCR0mhvbIs2E
               nNjWySh29zYFGnIK25KzY1Nkdziptzc2BKJUu7Qbm5sicQom2o3NzZEKqiu/DZpbmyIjIAHNBMZ
               x4iTALjhcgVQSIl3v87w5vePcY/AQYAFYR6skFSqBUAAAAASUVORK5CYII="
              alt="小米闪购"
            />
          </div>
          <div class="text">距离结束还有</div>
          <div class="time">
            <span class="time-box hour">00</span>
            <span class="rune">:</span>
            <span class="time-box minute">05</span>
            <span class="rune">:</span>
            <span class="time-box second">46</span>
          </div>
        </div>
        <div class="good-card" v-for="index in 4" :key="index">
          <div class="card-img">
            <img src="@/assets/ipad.png" alt />
          </div>
          <div class="name">小米米家液晶小黑板 13.5英寸</div>
          <div class="comment">随想随画 记录灵感瞬间</div>
          <div class="price">
            <span class="now-p">89</span>
            <span class="ori-p">99</span>
          </div>
        </div>
      </div>
      <div class="ad">
        <img
          data-src="//cdn.cnbj1.fds.api.mi-img.com/mi-mall/b6c7f2ccfb6b0e1a8a8aaa20ddba2322.jpg?thumb=1&amp;w=1839&amp;h=180&amp;f=webp&amp;q=90"
          src="//cdn.cnbj1.fds.api.mi-img.com/mi-mall/b6c7f2ccfb6b0e1a8a8aaa20ddba2322.jpg?thumb=1&amp;w=1839&amp;h=180&amp;f=webp&amp;q=90"
        />
      </div>
      <div class="shangou">
        <div class="gou-text">手机</div>
        <div class="more-arrow">
          查看全部
          <img src="@/assets/icon/lArrow.png" alt />
        </div>
      </div>
      <div class="divice">
        <div class="good-box">
          <div v-for="index in 2" :key="index">
            <div class="goodcard" v-for="index in 4" :key="index">
              <div class="good-img">
                <img src="@/assets/phone.png" alt />
              </div>
              <div class="good-name">小米10 青春版 5G</div>
              <div class="good-comment">50倍潜望式变焦/轻薄5G手机</div>
              <div class="good-price">
                <span class="now-p">3999 起</span>
                <span class="ori-p"></span>
              </div>
            </div>
          </div>
        </div>
        <div class="ad-div">
          <img
            alt
            data-src="//cdn.cnbj1.fds.api.mi-img.com/mi-mall/574c6643ab91c6618bfb2d0e2c761d0b.jpg?thumb=1&amp;w=351&amp;h=921&amp;f=webp&amp;q=90"
            src="//cdn.cnbj1.fds.api.mi-img.com/mi-mall/574c6643ab91c6618bfb2d0e2c761d0b.jpg?thumb=1&amp;w=351&amp;h=921&amp;f=webp&amp;q=90"
          />
        </div>
      </div>
      <div style="heigh:100px;width:100%"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      SL: [
        //   soft-list
        {
          text: "小米手机"
        },
        {
          text: "Redmi红米"
        },
        {
          text: "电视"
        },
        {
          text: "笔记本"
        },
        {
          text: "家电"
        },
        {
          text: "路由器"
        },
        {
          text: "智能硬件"
        },
        {
          text: "服务"
        },
        {
          text: "社区"
        }
      ],
      list: [
        {
          text: "手机 电话卡"
        },
        {
          text: "电视 盒子"
        },
        {
          text: "笔记本 显示器 平板"
        },
        {
          text: "家电 插线板"
        },
        {
          text: "出行 穿戴"
        },
        {
          text: "智能 路由器"
        },
        {
          text: "电源 配件"
        },
        {
          text: "健康 儿童"
        },
        {
          text: "耳机 音箱"
        },
        {
          text: "生活 箱包"
        }
      ]
    };
  }
};
</script>

<style lang="less">
.home {
  text-align: left;
  width: 100%;
  margin: 0 auto;
  background: red;


  .banner {
    width: 100%;
    padding: 0 10px;
    height: 300px;
    box-sizing: border-box;
    margin: 100px 0;
    margin-bottom: 40px;
    .ban-box {
      width: 100%;
      margin: auto;
      position: relative;
      height: 430px;
      margin-bottom: 20px;
      background: rgb(255, 255, 200);
      .dots {
        text-align: right;
        height: 10px;
        // width: 15%;
        position: absolute;
        bottom: 0px;
        right: 5px;
        z-index: 10;
        // background: chartreuse;
        .dot-box {
          margin: 0 5px;
          .dot {
            width: 7px;
            height: 7px;
            border-radius: 100%;
            background: rgb(126, 125, 125);
            border: 2px solid rgb(162, 160, 160);
            &:hover {
              background: rgb(216, 216, 216);
            }
          }
        }
      }
      .ban-img {
        width: 100%;
        height: 300px;
        position: relative;
        .l-arrow {
          position: absolute;
          top: 60%;
          margin-left: 20%;
          z-index: 10;
          left: 0px;
          font-size: 20px;
          padding: 20px 10px;
          &:hover {
            background: rgba(162, 160, 160, 0.6);
            color: white;
          }
        }
        .r-arrow {
          position: absolute;
          top: 60%;
          z-index: 10;
          right: 0px;
          font-size: 20px;
          padding: 20px 10px;
          &:hover {
            background: rgba(162, 160, 160, 0.6);
            color: white;
          }
        }
      }
      .ban-list {
        width: 20%;
        padding: 20px 0;
        box-sizing: border-box;
        background: rgb(162, 160, 160);
        font-size: 14px;
        position: absolute;
        top: 0;
        li {
          padding: 12px 0;
          padding-left: 12px;
          box-sizing: border-box;
          &:hover {
            background: rgb(255, 103, 0);
            border: 1px solid rgb(162, 160, 160);
            border-left: none;
            border-right: none;
          }
        }
        .list-item {
          color: white;
          padding: 0 20px;
          .more {
            margin-right: 20px;
          }
        }
      }
    }
    .ad-box {
      width: 100%;
      margin: auto;
      position: relative;
      margin-top: 60px;
      height: 180px;
      background: rgb(204, 248, 235);
      .func-btn {
        width: 20%;
        background: rgb(95, 87, 80);
        display: inline-block;
        padding: 5px;
        height: 180px;
        box-sizing: border-box;

        .func-td {
          width: 33%;
        }
        .btn {
          width: 100%;
          padding: 5px;
          padding-bottom: 0;
          box-sizing: border-box;
          border: 1px solid rgb(134, 134, 134);
          border-bottom: none;
          color: rgb(162, 160, 160);
          //   border: 3px solid rgb(139, 174, 238);
          //   background: rgb(230, 133, 133);
          font-size: 14px;
          position: relative;
          img {
            width: 40px;
            // margin: auto;
            margin-left: 10px;
            // margin-top: 5px;
          }
          p {
            margin-left: 5px;
            margin-top: 0px;
          }
          .block-tl {
            border-top: 1px solid rgb(95, 87, 80);
            border-left: 1px solid rgb(95, 87, 80);

            position: absolute;
            width: 15px;
            height: 15px;
            top: -1px;
            left: -1px;
          }
          .block-tr {
            border-top: 1px solid rgb(95, 87, 80);
            border-right: 1px solid rgb(95, 87, 80);

            position: absolute;
            width: 15px;
            height: 15px;
            top: -1px;
            right: -1px;
          }
          .block-bl {
            border-bottom: 1px solid rgb(95, 87, 80);
            border-left: 1px solid rgb(95, 87, 80);

            position: absolute;
            width: 15px;
            height: 15px;
            bottom: -1px;
            left: -1px;
          }
          .block-br {
            border-bottom: 1px solid rgb(95, 87, 80);
            border-right: 1px solid rgb(95, 87, 80);

            position: absolute;
            width: 15px;
            height: 15px;
            bottom: -1px;
            right: -1px;
          }
          &:hover {
            color: white;
          }
        }
        .bot-line {
          border-bottom: 1px solid rgb(162, 160, 160);
        }
      }
      .img-box {
        position: absolute;
        // background: red;
        width: 80%;
        top: 0;
        left: 21%;
        margin-left: 10px;
        .func-img {
          width: 31%;
          margin: 0 1%;
          box-sizing: border-box;
          height: 180px;
          &:hover {
            box-shadow: 0 20px 30px rgb(199, 199, 199);
          }
        }
      }
    }
  }
  .shop-cards {
    width: 100%;
    padding: 0 10px;
    // height: 300px;
    box-sizing: border-box;
    margin-top: 400px;
    background: rgb(245, 245, 245);
    .shangou {
      width: 100%;
      margin: 0 auto;
      height: 30px;
      position: relative;
      padding-top: 20px;
      .gou-text {
        position: absolute;
        font-size: 20px;
      }
      .arrow-box {
        position: absolute;
        right: 0;
        top: 20px;
        color: rgb(162, 160, 160);
        .arrow {
          padding: 5px;
          border: 1px solid rgb(199, 199, 199);
        }
        .arrow-r {
          border-left: none;
        }
      }
      .more-arrow {
        position: absolute;
        right: 0;
        font-size: 16px;

        img {
          float: right;
          width: 15px;
          height: 15px;
          padding: 5px;
          margin-left: 5px;
          border-radius: 100%;
          background: rgb(107, 107, 107);
        }
      }
    }
    .card-box {
      width: 100%;
      margin: 20px auto;
      height: 400px;
      position: relative;
      .card {
        float: left;
        width: 20%;
        background: rgb(241, 237, 237);
        height: 350px;
        border: 1px solid rgb(247, 231, 231);
        border-top: 1px solid red;
        padding: 50px 0;
        box-sizing: border-box;
        .changci {
          font-size: 22px;
          color: rgb(238, 58, 59);
          width: 35%;
          margin: auto;
        }
        .flash {
          width: 15%;
          margin: 30px auto;
        }
        .text {
          font-size: 16px;
          width: 40%;
          margin: 30px auto;
          color: rgb(111, 109, 109);
        }
        .time {
          width: 70%;
          margin: auto;
          margin-top: 30px;
          //   background: rgb(253, 108, 11);
          .time-box {
            font-size: 24px;
            padding: 10px;
            background: rgb(96, 87, 81);
            color: white;
          }
          .rune {
            width: auto;
            padding: 0 5px;
            font-size: 20px;
            font-weight: bold;
          }
        }
      }
      .good-card {
        float: right;
        width: 19%;
        margin-left: 1%;
        background: rgb(250, 250, 250);
        height: 350px;
        border: 1px solid rgb(247, 231, 231);
        border-top: 1px solid red;
        padding: 50px 0;
        box-sizing: border-box;
        .card-img {
          margin: auto;
          width: 50%;
        }
        .name {
          margin-top: 20px;
          font-size: 14px;
          text-align: center;
        }
        .comment {
          margin-top: 5px;
          color: rgb(187, 185, 185);
          font-size: 10px;
          text-align: center;
        }
        .price {
          text-align: center;
          .now-p {
            color: rgb(255, 103, 0);
          }
          .ori-p {
            margin-left: 10px;
            padding-top: 20px;
            color: rgb(187, 185, 185);
            text-decoration: line-through;
          }
        }
      }
    }
    .ad {
      width: 100%;
      height: 120px;
      margin: 0 auto;
      img {
        width: 100%;
      }
    }
    .divice {
      width: 100%;
      height: 600px;
      margin: 0 auto;
      margin-top: 10px;
      //   padding: 15px 0;
      box-sizing: border-box;
      //   background: red;
      .ad-div {
        width: 20%;
        height: 600px;
        img {
          width: 100%;
          height: 600px;
        }
        &:hover {
          margin-top: -1px;
          box-shadow: 0 20px 30px rgb(194, 194, 194);
        }
      }
      .good-box {
        float: right;
        width: 80%;
        // background: red;
        height: 600px;

        .goodcard {
          float: right;
          width: 23%;
          background: rgb(255, 255, 255);
          height: 290px;
          margin: 5px 5px;
          box-sizing: border-box;
          border: 1px solid rgb(247, 231, 231);
          //   border-top: 1px solid red;
          padding: 20px 0;
          box-sizing: border-box;
          .good-img {
            margin: auto;
            width: 50%;
            // background: red;
            img {
              width: 100%;
            }
          }
          .good-name {
            margin-top: 20px;
            font-size: 14px;
            text-align: center;
          }
          .good-comment {
            margin-top: 5px;
            color: rgb(187, 185, 185);
            font-size: 10px;
            text-align: center;
          }
          .good-price {
            margin-top: 10px;
            text-align: center;
            .now-p {
              color: rgb(255, 103, 0);
            }
            .ori-p {
              margin-left: 10px;
              padding-top: 20px;
              color: rgb(187, 185, 185);
              text-decoration: line-through;
            }
          }
          &:hover {
            // margin-top: 4px;
            box-shadow: 0 20px 30px rgb(194, 194, 194);
          }
        }
      }
    }
  }
}

.fl {
  float: left;
}
.fr {
  float: right;
}
li {
  list-style: none;
}
</style>