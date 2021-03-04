<template>
  <section id="home-container">
    <div id="home-content">
      <h1 id="home"> <span>I build responsive web applications</span> <br class="hide-laptop"></h1>
      <p>I'm Richard van Brunschot and I enjoy creating things that live on the internet, whether that be websites, applications, or anything in between.</p>
      <a v-scroll-to="'#projects-container'" class="button-link">View projects<i class="fas fa-chevron-down"></i></a>
      <img src="../assets/hero_landing.png" alt="Hero-landing">
    </div>
  </section>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #333;
$accent-color: #4d6bd8;


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

  .hide-laptop {
    display: none;
  }

    h1 {
      color: #111;
      width: 100%;
      font-family: 'Inter', sans-serif;
      font-size: 3rem;
      position: relative;
      max-width: 20ch;
      line-height: 1;
      font-weight: 400;
    }

    span {
      color: $accent-color;
      font-weight: 700;
    }

    p {
      color: #333;
      width: 45ch;
      font-family: 'Inter', sans-serif;
      font-size: 17px;
      margin-top: 1.75rem;
      font-weight: 500;
      line-height: 1.5;
    }

    .button-link {
      border: none;
      border-radius: 10px;
      background-color: $accent-color;
      color: $background-color;
      padding: 1rem 2rem;
      cursor: pointer;
      font-family: 'Inter', sans-serif;
      font-weight: bold;
      font-size: 1rem;
      margin-top: 3rem;
      text-decoration: none;
      transition: 0.25s ease;
      width: 200px;

      &:hover {
        background-color: #6f86db;

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
@media screen and (min-width: 1050px) and (max-width: 1600px) {
   #home-container {
    padding: 0 2rem;

    .hide-laptop {
      display: none;
    }

    #home-content {
      padding-top: 12.5rem;
    }

    img {
      width: 497px;
      height: 203px;
    }
  } 
}

// Smartphone
@media screen and (max-width: 700px) {

  #home-container {
    padding: 0 2rem;

    #home-content {
      padding-top: 10rem;

      h1 {
        font-size: 2.5rem;
        line-height: 1;
      }

      p {
        font-size: 1.2rem;
        margin-top: 2rem;
        width: 100%;
      }

      .button-link {
        margin-top: 3.5rem;
      }
    }

    img {
      display: none;
    }
  }
}

// Tablet
@media screen and (min-width: 701px) and (max-width: 1049px) {

  #home-container {
    padding: 0 2rem;

    #home-content {
      padding-top: 15rem;

      h1 {
        font-size: 3.5rem;
      }

      p {
        font-size: 1.25rem;
        margin-top: 5rem;
      }

      .button-link {
        margin-top: 3.5rem;
        font-size: 1.25rem;
        width: 200px;
        padding: 1rem;
      }
    }
  }
}
</style>
