
<!-- HTML -->

<template>
  <div id="app">
    <Nav />
    <HelloWorld msg="Octopy is your data butler!"/>
    <Button />
  </div>
</template>

<!-- JS -->
<script>
import HelloWorld from './components/HelloWorld.vue'
import Button from './components/Button.vue'
import Nav from './components/Nav.vue'


export default {
  name: 'App',
  components: {
    Nav,
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

body {
  background-color: #16171B;
 }

#app {
  font-family: var(--font-family);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--white);
}

</style>