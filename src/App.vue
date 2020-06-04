<template>
  <div id="app" class="center">
    <plateform></plateform>
  </div>
</template>

<script>
import plateform from "@/views/plateform.vue";

export default {
  name: "App",
  components: {
    plateform
  }
};
</script>

<style>
#app {
  font-family: Helvetica Neue, Helvetica, Arial, Microsoft Yahei,
    Hiragino Sans GB, Heiti SC, WenQuanYi Micro Hei, sans-serif;
  text-align: center;
  color: #2c3e50;
}
html,
body {
  width: 100%;
  height: 100vh;
  padding: 0;
  margin: 0;
  /* overflow-y: scroll; */
  /* overflow-x: hidden; */
}
.center {
  width: 1440px;
  margin: auto;
}
</style>
