<template>
  <div id="app">
    <Navbar></Navbar>
    <Home></Home>
    <Projects></Projects>
    <About></About>
    <Contact></Contact>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import Projects from './components/Projects.vue'
import About from './components/About.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Projects,
    About,
    Contact
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

@font-face {
  font-family: 'Calibre';
  src: url('../src/assets/CalibreRegular.woff') format('woff');
  font-weight: 500;
}

@font-face {
  font-family: 'Calibre';
  src: url('../src/assets/CalibreBold.woff') format('woff');
  font-weight: 700;
}

@font-face {
  font-family: 'Calibre';
  src: url('../src/assets/CalibreLight.woff') format('woff');
  font-weight: 300;
}

@font-face {
  font-family: 'Calibre';
  src: url('../src/assets/CalibreMedium.woff') format('woff');
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
