<template>
  <div>
    <h2 v-if="num === 0">The number is zero</h2>
    <h2 v-else-if="num < 0">The number is negative</h2>
    <h2 v-else-if="num > 0">The number is positive</h2>
    <h2 v-else>Not a number</h2>
    <template v-if="display">
      <h2>Aashay Kadu</h2>
      <h2>Codevolution</h2>
      <h2>Vue</h2>
    </template>
    <h2 v-show="showElement">Using v-show</h2>
    <!-- v-show will be always rendered to the dom -->
    <h2 v-if="showElement">Using v-if</h2>
    <!-- v-if will only rendered to the dom if condition is satisfied -->
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      num: "0",
      display: true,
      showElement:true,
    };
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
