<template>
  <div class="soft-box">
    <div class="soft-img">
      <div class="box">
        <img src="@/assets/icon/xiaomi.png" alt width="30px" />
      </div>
    </div>
    <div class="soft-list">
      <span v-for="(item,index) in SL" :key="index">
        <span class="list-text">{{item.text}}</span>
      </span>
    </div>
    <div class="soft-search">
      <div class="re">
        <img class="img" src="@/assets/icon/search-b.png" alt />
        <input class="input" type="text" placeholder="小米10 青春版" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "softlist",
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
      ]
    };
  }
};
</script>

<style lang="less">
.soft-box {
  width: 100%;
  margin: 10px 0;
  position: relative;
  
  .soft-img {
    width: 20%;
    height: 60px;
    position: absolute;
	// background: green;
	text-align: center;
    .box {
      width: 60px;
      height: 60px;
      background: rgb(255, 103, 0);
      img {
        height: 30px;
        margin: 15px auto;
      }
    }
  }
  .soft-list {
    position: absolute;
    left: 20%;
    width: 55%;
    font-size: 16px;
    top: 20px;
    z-index: 10;
    // background: rgb(197, 255, 197);
    .list-text {
      margin: auto 10px;
      &:hover {
        color: rgb(255, 103, 0);
      }
    }
  }
  .soft-search {
    position: absolute;
    right: 0;
    width: 25%;
    height: 60px;
    box-sizing: border-box;
    // background: rgb(179, 179, 252);
    .re {
      position: relative;
      .input {
        width: 95%;
        border: none;
        border: 1px solid rgb(224, 224, 224);
        height: 60px;
        padding: 10px;
        box-sizing: border-box;
        margin-left: 15px;
        outline: rgb(224, 224, 224);
        // color: rgb(224, 224, 224);
        &:focus {
          border: 1px solid rgb(255, 103, 0);
          outline: rgb(255, 103, 0);
        }
      }
      .img {
        position: absolute;
        top: 0px;
        right: 0;
        width: 59px;
        height: 59px;
        padding: 15px;
        box-sizing: border-box;
        border-left: 1px solid rgb(224, 224, 224);
        &:focus {
          border: 1px solid rgb(255, 103, 0);
          outline: rgb(255, 103, 0);
        }
      }
    }
  }
}
</style>