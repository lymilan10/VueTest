<template>
  <div id="app">
    <h1>Vue入口</h1>
    <father-a></father-a>
    <father-b></father-b>
    <father-c></father-c>
    <next-tick></next-tick>
  </div>
</template>
<script>
import FatherA from "./views/FatherA";
import FatherB from "./views/FatherB"
import FatherC from "./views/FatherC"
import NextTick from "./components/NextTick"

export default {
  components: {
    FatherA,FatherB,FatherC,NextTick
  },
};
</script>
<style lang="stylus">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
