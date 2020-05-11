<template>
  <div id="home-container">
    <div id="home-content">
      <h1 id="home">I create responsive and easy-to-use <br> websites.</h1>
      <p>My name is <span>Richard van Brunschot</span> and I'm a <span>Front-end Developer</span>,<br>
based in Veldhoven, The Netherlands.</p>
      <a href="#projects"><button class="button-link">See My Work <i class="fas fa-chevron-down"></i></button></a>
      <img src="../assets/hero_landing.png" alt="Hero-landing">
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #333;
$accent-color: #038AFF;

:target {
  padding-top: 240px;
  margin-top: -240px;
  display: inline-block;
}

// Default
#home-container {
  max-width: 1050px;
  height: 100vh;
  position: relative;
  margin: 0 auto;

  #home-content {
  display: flex;
  flex-direction: column;
  padding-top: 15rem;
  height: 100%;
  position: relative;

    a {
      width: 194px;
      height: 50px;
    }

    h1 {
      color: $text-color;
      width: 100%;
      font-family: 'SF', sans-serif;
      font-weight: bold;
      font-size: 3.75rem;
      position: relative;
    }

    p {
      color: $text-color;
      width: 100%;
      font-family: 'Calibre', sans-serif;
      font-size: 1.5rem;
      margin-top: 5rem;
      font-weight: 500;

      span:nth-child(2) {
        color: $accent-color;
      }
    }

    .button-link {
      border: none;
      border-radius: 10px;
      background-color: $accent-color;
      color: $background-color;
      padding: 1rem 2rem;
      cursor: pointer;
      font-family: 'SF', sans-serif;
      font-weight: bold;
      font-size: 1rem;
      margin-top: 5rem;
      text-decoration: none;
      transition: 0.25s ease;

      &:hover {
        background-color: rgb(43, 156, 255);

        i {
          transform: translateY(5px)
        }
      }

      i {
        margin-left: 10px;
        font-size: 1.1rem;
        transition: 0.25s ease;
      }
    }
  }

    img {
      position: absolute;
      bottom: 0;
      right: 0;
      width: 608px;
      height: 248px;
    }
}

// Laptop
@media screen and (min-width: 1101px) and (max-width: 1500px) {
  
}

// Smartphone
@media screen and (max-width: 450px) {
  #home-container {
    padding: 0 2rem;

    #home-content {
      padding-top: 10rem;

      h1 {
        font-size: 2.5rem;
      }

      p {
        font-size: 1.35rem;
        margin-top: 5rem;
      }
    }

    img {
      display: none;
    }
  }
}

// Tablet
@media screen and (min-width: 451px) and (max-width: 1100px) {
  #home-container {
    padding: 0 2rem;

    #home-content {
      padding-top: 10rem;

      h1 {
        font-size: 2.5rem;
      }

      p {
        font-size: 1.35rem;
        margin-top: 5rem;
      }
    }

    img {
      display: none;
    }
  }
}
</style>
