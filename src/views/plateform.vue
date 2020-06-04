<template>
  <div class="plateform">
    <div class="header">
      <headerbar></headerbar>
    </div>

    <div class="center sl">
      <softlist></softlist>
    </div>
    <div class="center ba">
      <banner class="banner"></banner>
    </div>
    <div class="center sc">
      <shopcard></shopcard>
    </div>
  </div>
</template>

<script>
import headerbar from "@/components/headerbar.vue";
import softlist from "@/components/softlist.vue";
import banner from "@/components/banner.vue";
import shopcard from "@/components/shopcard.vue";
export default {
  name: "plateform",
  components: {
    headerbar,
    softlist,
    banner,
    shopcard
  }
};
</script>

<style lang="less">
.plateform {
//   width: 100%;
  min-width: 1226px;
//   background: rgb(255, 218, 218);
  text-align: left;
  .header {
	width: 100%;
	height: 40px;
	background: rgb(51, 51, 51);
  }
  .center {
    width: 1226px;
    margin: 0 auto;
    // background: rgb(255, 240, 220);
  }
  .sl {
    // background: rgb(255, 240, 220);
    height: 60px;
  }
  .ba {
    // background: rgb(177, 210, 253);
    height: 700px;
    z-index: 10;
  }
  .sc {
    // background: rgb(253, 177, 212);
    height: 500px;
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