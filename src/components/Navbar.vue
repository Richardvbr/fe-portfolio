<template>
  <nav id="nav-container">
    <div class="logo">
      <a v-scroll-to="'#home-container'"><img src="../../public/android-chrome-192x192.png" alt="Logo"></a>
    </div>
    <ul>
      <li><a v-scroll-to="'#projects-container'">Projects</a></li>
      <li><a v-scroll-to="'#skillset-container'">Skills</a></li>
      <li><a v-scroll-to="'#contact-container'">Contact</a></li>
      <li><a href="https://github.com/Richardvbr" target="_blank" class="github-link">GitHub</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #333;
$accent-color: #4d6bd8;

#nav-container {
  background-color: #fff;
  width: 100vw;
  height: 4rem;
  box-shadow: 0px 8px 15px 1px rgba(0,0,0,0.13);
  position: fixed;
  top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 10rem;
  z-index: 1;

  .logo img {
    max-width: 45px;
    transition: 0.2s ease;
    // Hide jagged edges
    outline: 1px solid transparent;
  }

  ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
    list-style: none;

    li a {
      text-decoration: none;
      color: $text-color;
      font-family: 'Inter', sans-serif;
      font-weight: 700;
      padding: 0.5rem 1.5rem;
      transition: 0.25s ease;
    
      &:hover {
        color: $accent-color;
      }
    }
  }
    .github-link {
      color: $accent-color;
    }
}

// Smartphone
@media screen and (max-width: 700px) {
  #nav-container {
  padding: 0 2rem;
  align-items: center;
  justify-content: center;
  flex-direction: row;
  height: 4rem;

  .logo img {
    max-width: 35px;
    margin: 0.5rem;
  }

  ul {
    display: flex;
    padding: 0;
    li a {
      padding: 0.5rem 0.75rem;
    }
  }

    .resume-link {
      display: none;

    }
  }
}

// Tablet
@media screen and (min-width: 701px) and (max-width: 1049px) {
  #nav-container {
  padding: 0 2rem;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  height: 6rem;
  width: 100%;

  .logo img {
    max-width: 35px;
    margin: 0.5rem;
  }

  ul {
    font-size: 1.25rem;
    display: flex;
    padding: 0 0 1rem 0;
    li a {
      padding: 0.5rem 1rem;
    }
  }

    .resume-link {
      display: none;
    }
  }
}

</style>
