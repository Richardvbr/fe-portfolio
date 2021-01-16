<template>
  <div id="app">
    <Navbar></Navbar>
    <Home></Home>
    <Projects></Projects>
    <Skillset></Skillset>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'
import Projects from './components/Projects.vue'
import Skillset from './components/Skillset.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Projects,
    Skillset,
    Contact,
    Footer
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap');

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
