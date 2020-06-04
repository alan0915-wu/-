<template>
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
        <div class="btn-box">
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
</template>

<script>
export default {
  name: "banner",
  data() {
    return {
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
.banner {
  width: 100%;
  height: 300px;
  box-sizing: border-box;
  margin: auto;
  margin-top: 20px;
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

      .btn-box {
        margin: auto;
        .func-td {
          width: 30%;
          margin: 0 1%;
          .btn {
            width: 100%;
            padding: 5px;
            padding-bottom: 0;
            box-sizing: border-box;
            border: 1px solid rgb(126, 126, 126);
            border-bottom: none;
            color: rgb(162, 160, 160);
            font-size: 14px;
            position: relative;
            text-align: center;
            img {
              width: 40px;
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
      }
    }
    .img-box {
      position: absolute;
      text-align: right;
      width: 81%;
      top: 0;
      right: 0;
      margin-left: 10px;
      .func-img {
        width: 30%;
        // margin: 0 1%;
        margin-left: 3%;
        box-sizing: border-box;
        height: 180px;
        &:hover {
          box-shadow: 0 20px 30px rgb(199, 199, 199);
        }
      }
    }
  }
}
</style>