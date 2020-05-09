<template>
  <nav id="nav-container" class="anchor">
    <div class="logo">
      <a href="#home"><img src="../../public/android-chrome-192x192.png" alt="Logo"></a>
    </div>
    <ul>
      <li><a href="#projects">Projects</a></li>
      <li><a href=#about>About</a></li>
      <li><a href=#contact>Contact</a></li>
      <li><a href='/resume.pdf' target="blank" class="resume-link">Resume</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #333;
$accent-color: #038AFF;

#nav-container {
  background-color: #fff;
  width: 100vw;
  height: 4.5rem;
  box-shadow: 0px 10px 15px 1px rgba(0,0,0,0.2);
  position: fixed;
  top: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 5rem;
  z-index: 1;

  .logo img {
    max-width: 45px;
    transition: 0.2s ease;
    // Hide jagged edges
    outline: 1px solid transparent;

    &:hover {
      transform: scale(1.1) rotate(-15deg);
    }
  }

  ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
    list-style: none;

    li a {
      text-decoration: none;
      color: $text-color;
      font-family: 'SF', sans-serif;
      font-weight: bold;
      padding: 0.5rem 1.5rem;
      transition: 0.25s ease;
    
      &:hover {
        color: $accent-color;
      }
    }
  }

    .resume-link {
      color: $accent-color;
      border: solid 2px $accent-color;
      border-radius: 10px;
      padding: 0.5rem 1rem;
      margin-left: 1rem;

      &:hover {
        color: $background-color;
        background-color: $accent-color;
      }
    }
}

</style>
