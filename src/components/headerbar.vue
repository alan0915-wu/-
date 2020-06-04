<template>
  <div class="head-bar">
    <div class="head-box">
      <div class="list">
        <span class="select-list" v-for="(item,index) in HB" :key="index">
          <span class="bar-text">{{item.text}}</span>
          <span class="bar-div" v-if="item.end == '1'?false:true">|</span>
        </span>
      </div>

      <span class="func-list">
        <span class="fl">
          <span class="bar-text">登录</span>
          <span class="bar-div">|</span>
          <span class="bar-text">注册</span>
          <span class="bar-div">|</span>
          <span class="bar-text">消息通知</span>
        </span>

        <span class="shop-car">
          <img class="car-icon" src="@/assets/icon/cart.png" alt width="100%" />
          <span class="car-text">购物车</span>
          <span class="car-num">(0)</span>
        </span>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "header",
  data() {
    return {
      HB: [
        // headbar
        {
          text: "小米商城"
        },
        {
          text: "MIUI"
        },
        {
          text: "loT"
        },
        {
          text: "云服务"
        },
        {
          text: "金融"
        },
        {
          text: "有品"
        },
        {
          text: "小爱开发平台"
        },
        {
          text: "企业团购"
        },
        {
          text: "资质证照"
        },
        {
          text: "协议规则"
        },
        {
          text: "下载app"
        },
        {
          text: "Select Location",
          end: 1
        }
      ]
    };
  }
};
</script>

<style lang="less">
.head-bar {
  width: 100%;
  max-width: 1226px;
  margin:0 auto;
  background: rgb(51, 51, 51);
  .head-box {
    width: 100%;
    // margin: auto;
    height: 40px;
    padding: 10px 0;
    box-sizing: border-box;
    color: #b0b0b0;
    font-size: 12px;
    position: relative;

    .bar-text {
      margin: auto;
      padding: 0 5px;
      &:hover {
        color: white;
      }
    }
    .bar-div {
      color: rgb(65, 65, 65);
    }
    .shop-car {
      padding: 10px 30px;
      height: 40px;
      box-sizing: border-box;
      position: relative;
      background: rgb(61, 61, 61);
      .car-icon {
        width: 15px;
        margin-right: 10px;
        position: absolute;
        top: 10px;
        left: 10px;
      }
      .car-text {
        margin: 0 2px;
        // position: absolute;
      }
      .car-num {
        top: 10px;
        position: absolute;
      }
    }
    .list {
      //   background: red;
      position: absolute;
      left: 0%;
    }
    .func-list {
      position: absolute;
      right: 0%;
    }
  }
}
</style>