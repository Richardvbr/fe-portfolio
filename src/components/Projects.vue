<template>
  <div id="projects-container">
    <h2 id="projects">Projects</h2>
    <div id="container-3d">
      <div class="left-3d">
        <div class="image-3d">
          <a href="https://richardvbr-3d-vue.netlify.com/" target=”_blank” rel=”noreferrer“><img src="../assets/hero_3d.jpg" alt="3d modeling portfolio"></a>
        </div>
      </div>
      <div class="right-3d">
        <h3>{{ portfolio3d.title }}</h3>
        <p class="portfolio3d-description">{{ portfolio3d.description }}</p>
        <p class="portfolio3d-software">{{ portfolio3d.software }}</p>
        <div class="links-buttons right-side">
          <a href="https://richardvbr-3d-vue.netlify.com/" target=”_blank” rel=”noreferrer“><button class="button-link">Live Website <i class="fas fa-external-link-alt"></i></button></a>
          <a href="https://github.com/Richardvbr/3d-portfolio-vue" target=”_blank” rel=”noreferrer“><button class="button-link">View Code <i class="fas fa-external-link-alt"></i></button></a>
        </div>
      </div>
    </div>
    <div id="container-weather">
      <div class="right-weather">
        <h3>{{ weatherapp.title }}</h3>
        <p class="weather-description">{{ weatherapp.description }}</p>
        <p class="weather-software">{{ weatherapp.software }}</p>
        <div class="links-buttons left-side">
          <a href="https://todays-weather-rvbr.herokuapp.com/" target=”_blank” rel=”noreferrer“><button class="button-link">Live Website <i class="fas fa-external-link-alt"></i></button></a>
          <a href="https://github.com/Richardvbr/Todaysweather" target=”_blank” rel=”noreferrer“><button class="button-link">View Code <i class="fas fa-external-link-alt"></i></button></a>
        </div>
      </div>
      <div class="right-weather">
        <div class="image-weather">
          <a href="https://todays-weather-rvbr.herokuapp.com/" target=”_blank” rel=”noreferrer“><img src="../assets/hero_weather.jpg" alt="3d modeling portfolio"></a>
        </div>
      </div>
    </div>
    <div id="container-frontend">
      <div class="left-frontend">
        <div class="image-frontend">
          <a href="https://richardvbr-3d-vue.netlify.com/" target=”_blank” rel=”noreferrer“><img src="../assets/hero_fe.png" alt="3d modeling portfolio"></a>
        </div>
      </div>
      <div class="right-frontend">
        <h3>{{ portfolio.title }}</h3>
        <p class="frontend-description">{{ portfolio.description }}</p>
        <p class="frontend-software">{{ portfolio.software }}</p>
        <div class="links-buttons right-side">
          <a href="https://richardvbr-3d-vue.netlify.com/" target=”_blank” rel=”noreferrer“><button class="button-link">Live Website <i class="fas fa-external-link-alt"></i></button></a>
          <a href="https://github.com/Richardvbr/3d-portfolio-vue" target="blank"><button class="button-link">View Code <i class="fas fa-external-link-alt"></i></button></a>
        </div>
      </div>
    </div>
    <div id="container-todo">
      <div class="right-todo">
        <h3>{{ todoapp.title }}</h3>
        <p class="todo-description">{{ todoapp.description }}</p>
        <p class="todo-software">{{ todoapp.software }}</p>
        <div class="links-buttons left-side">
          <a href="https://richardvbr-todoapp.netlify.com/" target=”_blank” rel=”noreferrer“><button class="button-link">Live Website <i class="fas fa-external-link-alt"></i></button></a>
          <a href="https://github.com/Richardvbr/Todo-app" target=”_blank” rel=”noreferrer“><button class="button-link">View Code <i class="fas fa-external-link-alt"></i></button></a>
        </div>
      </div>
      <div class="right-todo">
        <div class="image-todo">
          <a href="https://richardvbr-todoapp.netlify.com/" target=”_blank” rel=”noreferrer“><img src="../assets/hero_todo.jpg" alt="to-do app"></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data: function () {
    return  {
      portfolio3d: {
        title: '3D Modeling Portfolio',
        description: 'A nicer look at your GitHub profile and repo stats. Includes data visualizations of your top languages, starred repositories, and sort through your top repos by number of stars, forks, and size.',
        software: 'Vue.js, Vue Router, HTML5, SCSS, AdobeXD'
      },
      weatherapp: {
        title: 'Weather App',
        description: 'A nicer look at your GitHub profile and repo stats. Includes data visualizations of your top languages, starred repositories, and sort through your top repos by number of stars, forks, and size.',
        software: 'JavaScript, HTML5, SCSS, AdobeXD',
      },
      portfolio: {
        title: 'Front-end Portfolio',
        description: 'A nicer look at your GitHub profile and repo stats. Includes data visualizations of your top languages, starred repositories, and sort through your top repos by number of stars, forks, and size.',
        software: 'Vue.js, HTML5, SCSS, AdobeXD',
      },
      todoapp: {
        title: 'To-do App',
        description: 'A nicer look at your GitHub profile and repo stats. Includes data visualizations of your top languages, starred repositories, and sort through your top repos by number of stars, forks, and size.',
        software: 'JavaScript, HTML5, CSS',  
      }
    }
  }
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #333;
$accent-color: #038AFF;

// :target {
  // padding-top: 240px;
  // margin-top: -240px;
  // display: inline-block;
// }

#projects-container {
  max-width: 1050px;
  height: 100vh;
  position: relative;
  margin: 0 auto;
  font-family: 'SF', sans-serif;
  color: $text-color;

  .right-side {
    a {
      margin-left: 44px;
    }
  }

  .left-side {
    a {
      margin-right: 44px;
    }
  }

  img {
    max-width: 650px;
    box-shadow: 0px 0px 10px 10px rgba(0,0,0,0.1);
    transition: 0.25s ease;

    &:hover {
      transform: scale(1.005)
    }
  }

  h2 {
    padding-top: 6rem;
    font-family: 'SF', sans-serif;
    font-size: 2rem;
    margin-bottom: 2rem;
    color: $text-color;
  }

  a {
    font-family: 'SF', sans-serif;
  }

  .button-link {
    border: 2px solid $accent-color;
    border-radius: 13px;
    background-color: $background-color;
    color: $accent-color;
    padding: 0.6rem 1rem;
    cursor: pointer;
    font-weight: bold;
    font-size: 1rem;
    font-family: 'SF', sans-serif;
    transition: 0.25s ease;

    &:hover {
      color: $background-color;
      background-color: $accent-color;
    }

    i {
      margin-left: 10px;
    }
  }

  #container-3d {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    height: 320px;
    position: relative;

    .links-buttons {
      display: flex;
      position: absolute;
      bottom: 0;
      right: 0;
    }

    .right-3d {
      text-align: left;

      h3 {
        color: $accent-color;
        font-size: 1.75rem;
        text-align: right;
      }

      .portfolio3d-description,
      .portfolio3d-software {
        color: $text-color;
        font-size: 1.05rem;
      }

      .portfolio3d-description {
        padding-left: 40px;
        text-align: right;
        padding-top: 20px;
      }

      .portfolio3d-software {
        text-align: right;
        padding-top: 100px;
        font-weight: bold;
      }
    }
  }

  #container-weather {
    margin-top: 100px;
    margin-bottom: 100px;
    display: flex;
    width: 100%;
    height: 320px;
    justify-content: space-between;
    position: relative;

    .links-buttons {
      display: flex;
      position: absolute;
      bottom: 0;
      left: 0;
    }

    h3 {
      font-size: 2rem;
      color: $accent-color;
    }

    .weather-description,
    .weather-software {
      color: $text-color;
      font-size: 1.05rem;
    }

    .weather-description {
      padding-right: 40px;
      padding-top: 20px;
    }

    .weather-software {
      padding-top: 95px;
      font-weight: bold;
    }
  }

  #container-frontend {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    height: 320px;
    position: relative;

    img {
      height: 320px;
    }

    .links-buttons {
      display: flex;
      position: absolute;
      bottom: 0;
      right: 0;
    }

    .right-frontend {
      text-align: left;

      h3 {
        color: $accent-color;
        font-size: 1.75rem;
        text-align: right;
      }

      .frontend-description,
      .frontend-software {
        color: $text-color;
        font-size: 1.05rem;
      }

      .frontend-description {
        padding-left: 40px;
        text-align: right;
        padding-top: 20px;
      }

      .frontend-software {
        text-align: right;
        padding-top: 100px;
        font-weight: bold;
      }
    }
  }

  #container-todo {
    margin-top: 100px;
    margin-bottom: 100px;
    display: flex;
    width: 100%;
    height: 320px;
    justify-content: space-between;
    position: relative;

    .links-buttons {
      display: flex;
      position: absolute;
      bottom: 0;
      left: 0;
    }

    h3 {
      font-size: 2rem;
      color: $accent-color;
    }

    .todo-description,
    .todo-software {
      color: $text-color;
      font-size: 1.05rem;
    }

    .todo-description {
      padding-right: 40px;
      padding-top: 20px;
    }

    .todo-software {
      padding-top: 95px;
      font-weight: bold;
    }
  }
}
</style>
