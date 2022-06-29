<template>
  <div>
    <a @click="one" href="http://www.baidu.com">阻止百度</a>
    <hr />
    <a @click="two(10, $event)" href="http://www.baidu.com">阻止去百度</a>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {};
  },
  methods: {
    one(e) {
      e.preventDefault();
      console.log(1);
    },
    two(val, e) {
      e.preventDefault();
      console.log(2);
    },
  },
};
</script>

<style>
</style>