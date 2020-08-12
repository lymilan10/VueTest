<template>
  <div>
    <!-- 用ref给子组件起个名字 -->
    <child-b ref="child_b"></child-b>
    <button @click="getMyEvent">点击父组件B</button>
  </div>
</template>

<script>
import ChildB from '../components/ChildB'
export default {
  components: {
    ChildB,
  },
  data() {
    return {
      msg: "我是父组件B中的数据",
    };
  },
  methods:{
      getMyEvent(){
          this.$refs.child_b.emitEvent(this.msg);
      }
  }
};
</script>

<style>
</style>