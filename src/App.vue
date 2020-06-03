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
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 100;
  font-display: swap;
  src: url("../src/assets/Inter-Thin.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-Thin.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 200;
  font-display: swap;
  src: url("../src/assets/Inter-ExtraLight.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-ExtraLight.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 300;
  font-display: swap;
  src: url("../src/assets/Inter-Light.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-Light.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 400;
  font-display: swap;
  src: url("../src/assets/Inter-Regular.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-Regular.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 500;
  font-display: swap;
  src: url("../src/assets/Inter-Medium.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-Medium.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 600;
  font-display: swap;
  src: url("../src/assets/Inter-SemiBold.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-SemiBold.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 700;
  font-display: swap;
  src: url("../src/assets/Inter-Bold.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-Bold.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 800;
  font-display: swap;
  src: url("../src/assets/Inter-ExtraBold.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-ExtraBold.woff?v=3.13") format("woff");
}

@font-face {
  font-family: 'Inter';
  font-style:  normal;
  font-weight: 900;
  font-display: swap;
  src: url("../src/assets/Inter-Black.woff2?v=3.13") format("woff2"),
       url("../src/assets/Inter-Black.woff?v=3.13") format("woff");
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  body {
    background-color: #f7f7f7;
  }
}

a {
  cursor: pointer;
}

p {
  font-weight: 500;
  font-size: 17px;
  line-height: 1.4;
}
</style>
