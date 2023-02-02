<template>
  <div id="app">
    <child-component>
      <template #top="{ myUser }">{{ myUser }}</template>
      默认的slots
    </child-component>
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
