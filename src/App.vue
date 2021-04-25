<template>
  <div class="App">
    <div class="hello">Hello {{ who }}</div>
    <br>
    <div>{{setConfig}}</div>
    <p>
      <router-link to="/">Go To Home</router-link>
      <router-link to="/page2">Go To page2</router-link>
    </p>
    <router-view></router-view>
  </div>
</template>

<script>
module.exports = {
  data: function() {
    return {
      who: "Vue and Webpack !!",
      setConfig: CONFIG
    };
  },
  created() {
    console.log(CONFIG)
  },
};
</script>

<style scoped>
.hello {
  padding: 0.5em;
  font-size: 2em;
  background-color: #fcf;
}
</style>
