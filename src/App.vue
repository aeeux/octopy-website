
<!-- HTML -->

<template>
  <div id="app">
    <img id="logo" alt="Vue logo" src="./assets/octopy-logo.png">
    <HelloWorld msg="Octopy is your data butler!"/>
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
  },
}

</script>

<!-- CSS -->

<style>

:root {
    --lightblue: #44c1ed;
    --blue: #3185df;
    --darkblue: #4479ed;
    --offblue: #16171B;
    --offdark: #23272a;
    --white: whitesmoke;

    --font-family: 'Work Sans', sans-serif;
}

#logo {
  width: 10%;
  height: auto;
}

body {
  background-color: var(--offdark);
 }

#app {
  font-family: var(--font-family);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #16171B;
  margin-top: 60px;
}

</style>