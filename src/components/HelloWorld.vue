<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <alert mode="primary">First Alert</alert>
    <alert mode="danger">Second Alert</alert>
    <alert mode="success">Third Alert</alert>
    <alert mode="secondary">Last Alert</alert>
    
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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
