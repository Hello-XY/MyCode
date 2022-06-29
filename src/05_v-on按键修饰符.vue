<template>
  <div>
    <!-- 1. 绑定键盘按下事件.enter - 回车 
         2. .esc修饰符 - 取消键-->
    <input type="text" @keydown.enter="enterFn" />
    <hr />
    <input type="text" @keydown.esc="escFn" />
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {};
  },
  methods: {
    enterFn() {
      alert("按下了enter键");
    },
    escFn() {
      alert("按下了esc键");
    },
  },
};
</script>

<style>
</style>