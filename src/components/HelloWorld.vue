<template>
  <div class="menu">
    <ul>
      <li><a href="">Link1</a></li>
      <li><a href="">Link2</a></li>
      <li><a href="">Link3</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.menu ul li a {
  text-decoration: none;
  margin: 15px;
  font-family: "Courier New", Courier, monospace;
}
.menu ul li {
  display: inline-block;
  margin: 5px;
  border-radius: 2px;
  border-right: 1px solid silver;
  border-bottom: 1px solid black;
}
</style>
