<template>
  <div>
    
  </div>
</template>

<script>
export default {
  methods: {
    emitEvent(msg) {
      console.log("子组件B接收的数据----->" + msg);
    },
  },
};
</script>

<style>
</style>