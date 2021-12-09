<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <TextElements/>
  </div>
</template>

<script>
import TextElements from './components/TestElements.vue'

export default {
  name: 'App',
  components: {
    TextElements
  }
}
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
