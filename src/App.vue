<template>
  <el-container id="container">
    <el-header style="height: 120px">
      <el-col :span="12" class="nav-header"
        ><h1
          style="
            line-height: 1.5;
            font-size: 36px;
            color: #d4c7ce;
            text-align: left;
            text-shadow: black 0.1em 0.1em 0.2em;
          "
        >
          HEARTMEET
        </h1></el-col
      >
      <el-col :span="12" class="nav-header" style="">
        <span></span>
      </el-col>
    </el-header>
    <el-main>Main</el-main>
  </el-container>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      searchInput: "",
    };
  },
  mounted() {
    const h = this.$createElement;

    this.$notify({
      message: h(
        "i",
        { style: "color: teal" },
        "你好，欢迎来到心遇博客！美丽的心，终将会相遇！"
      ),
      duration: 3000,
      offset: 50,
    });
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  margin: 0;
  padding: 0;
  line-height: 1.5em;
  color: #000;
  font-size: 14px;
  font-family: "Helvetica Neue", "Helvetica", "PingFang SC", "Hiragino Sans GB",
    "Microsoft YaHei", "微软雅黑", "Arial", "sans-serif";
}
#container {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  min-width: 1000px;
  z-index: -10;
  zoom: 1;
  background: #fff url("../static/background.jpg") center 0 no-repeat;
  background-size: 100% 100%;
  -webkit-background-size: 100% 100%;
  -o-background-size: 100% 100%;
}
.nav-header {
  position: relative;
  top: 50%;
  margin-top: -10px;
}
</style>
