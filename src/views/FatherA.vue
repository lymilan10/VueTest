<template>
  <div>
      <child-a @my-event="getMyEvent"></child-a>
  </div>
</template>

<script>
import ChildA from "../components/ChildA";
export default {
  components: {
    ChildA,
  },
  methods: {
    getMyEvent(msg) {
      console.log("父组件A接收的数据----->" + msg);
    },
  },
};
</script>

<style>
</style>