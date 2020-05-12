<template>
  <div id="app">
    <Navbar></Navbar>
    <Home></Home>
    <Projects></Projects>
    <About></About>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import Projects from './components/Projects.vue'
import About from './components/About.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Projects,
    About,
    Contact,
    Footer
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

html {
  scroll-behavior: smooth;
  overflow-x: hidden;
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
