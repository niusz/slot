<template>
  <div class="hello">
    <slot>Some default message</slot>
    <br />
    <slot name="top" :myUser="user"></slot>
    <br />
    <slot name="bottom"></slot>
  </div>
</template>

<script>
export default {
  name: "ChildComponent",
  data() {
    return {
      user: "小狐狸",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
