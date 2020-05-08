<template>
  <div id="app">
    <Navbar></Navbar>
    <Home></Home>
    <Projects></Projects>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import Projects from './components/Projects.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Projects
  }
}
</script>

<style lang="scss">
@font-face {
  font-family: 'SF';
  src: url('../src/assets/SF-UI-Display-Bold.otf') format('otf');
  font-weight: 800;
}

@font-face {
  font-family: 'SF';
  src: url('../src/assets/SF-UI-Display-Medium.otf') format('otf');
  font-weight: 600;
}

html {
  scroll-behavior: smooth;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  body {
    background-color: #f7f7f7;
  }
}
</style>
