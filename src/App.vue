
<!-- HTML -->

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Button />
  </div>
</template>

<!-- JS -->

<script>
import HelloWorld from './components/HelloWorld.vue'
import Button from './components/Button.vue'

export default {
  name: 'App',
  components: {
    Button,
    HelloWorld
  }
}
</script>

<!-- CSS -->

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