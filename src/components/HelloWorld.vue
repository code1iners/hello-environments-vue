<template>
  <div class="hello">
    <div>{{ common }}</div>
    <div>{{ whoAmI }}</div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  setup() {
    const common = process.env.VUE_APP_COMMON;
    const whoAmI = process.env.VUE_APP_WHO_AM_I;
    return {
      common,
      whoAmI,
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
