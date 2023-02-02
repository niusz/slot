<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <child-component msg="Welcome to Your Vue.js App"></child-component>
    <!--如果HelloWorld中的没有slot元素，那么<h3>大标题</h3>将不会显示-->
  </div>
</template>

<script>
import ChildComponent from "./components/ChildComponent.vue";

export default {
  name: "App",
  components: {
    ChildComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
