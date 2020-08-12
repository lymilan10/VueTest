<template>
  <div>
    <button @click="emitEvent">点击子组件A</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "我是子组件A中的数据",
    };
  },
  methods: {
    emitEvent() {
      this.$emit("my-event", this.msg);
    },
  },
};
</script>

<style>
</style>