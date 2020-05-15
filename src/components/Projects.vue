<template>
  <div id="projects-container">
    <h2 id="projects">Projects</h2>
    <div id="container-3d" data-aos="fade-up" data-aos-delay="150">
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
          <a href="https://richardvbr-3d-vue.netlify.com/" target=”_blank” rel=”noreferrer“ class="button-link">Live Website <i class="fas fa-external-link-alt"></i></a>
          <a href="https://github.com/Richardvbr/3d-portfolio-vue" target=”_blank” rel=”noreferrer“ class="button-link">View Code <i class="fas fa-external-link-alt"></i></a>
        </div>
      </div>
    </div>
    <div id="container-weather" data-aos="fade-up" data-aos-delay="150">
      <div class="left-weather">
        <h3>{{ weatherapp.title }}</h3>
        <p class="weather-description">{{ weatherapp.description }}</p>
        <p class="weather-software">{{ weatherapp.software }}</p>
        <div class="links-buttons left-side">
          <a href="https://todays-weather-rvbr.herokuapp.com/" target=”_blank” rel=”noreferrer“ class="button-link">Live Website <i class="fas fa-external-link-alt"></i></a>
          <a href="https://github.com/Richardvbr/Todaysweather" target=”_blank” rel=”noreferrer“ class="button-link">View Code <i class="fas fa-external-link-alt"></i></a>
        </div>
      </div>
      <div class="right-weather">
        <div class="image-weather">
          <a href="https://todays-weather-rvbr.herokuapp.com/" target=”_blank” rel=”noreferrer“><img src="../assets/hero_weather.jpg" alt="3d modeling portfolio"></a>
        </div>
      </div>
    </div>
    <div id="container-frontend" data-aos="fade-up" data-aos-delay="150">
      <div class="left-frontend">
        <div class="image-frontend">
          <a href="https://www.brunschot.dev/" target=”_blank” rel=”noreferrer“><img src="../assets/hero_fe.jpg" alt="3d modeling portfolio"></a>
        </div>
      </div>
      <div class="right-frontend">
        <h3>{{ portfolio.title }}</h3>
        <p class="frontend-description">{{ portfolio.description }}</p>
        <p class="frontend-software">{{ portfolio.software }}</p>
        <div class="links-buttons right-side">
          <a href="https://www.brunschot.dev/" target=”_blank” rel=”noreferrer“ class="button-link">Live Website <i class="fas fa-external-link-alt"></i></a>
          <a href="https://github.com/Richardvbr/fe-portfolio" target="blank" class="button-link">View Code <i class="fas fa-external-link-alt"></i></a>
        </div>
      </div>
    </div>
    <div id="container-todo" data-aos="fade-up" data-aos-delay="150">
      <div class="left-todo">
        <h3>{{ todoapp.title }}</h3>
        <p class="todo-description">{{ todoapp.description }}</p>
        <p class="todo-software">{{ todoapp.software }}</p>
        <div class="links-buttons left-side">
          <a href="https://richardvbr-todoapp.netlify.com/" target=”_blank” rel=”noreferrer“ class="button-link">Live Website <i class="fas fa-external-link-alt"></i></a>
          <a href="https://github.com/Richardvbr/Todo-app" target=”_blank” rel=”noreferrer“ class="button-link">View Code <i class="fas fa-external-link-alt"></i></a>
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
        description: "Portfolio website to showcase 3D models. Vue.js single-page application to provide a performant and modern experience. New portfolio items are added to the grid automatically using JSON and for loops.",
        software: 'Vue.js, Vue Router, HTML5, SCSS, AdobeXD'
      },
      weatherapp: {
        title: 'Weather App',
        description: "Weather application that displays local current weather information. Fetches weather data using the Dark Sky API. API calls are done on a Node/Express back-end so that the API key is hidden and secured.",
        software: 'JavaScript, HTML5, SCSS, AdobeXD',
      },
      portfolio: {
        title: 'Front-end Portfolio',
        description: "Portfolio website to showcase my work as a front-end developer. Opted for a clean design that is easy on the eyes. Responsive design and scroll-based animations.",
        software: 'Vue.js, HTML5, SCSS, AdobeXD',
      },
      todoapp: {
        title: 'To-do App',
        description: "To-do application that utilizes the browser's Local Storage to remember your to-do lists. Shows current date and prevents empty inputs.",
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

#projects-container {
  max-width: 1050px;
  position: relative;
  margin: 0 auto;
  font-family: 'Calibre', sans-serif;
  font-size: 20px;  
  color: $text-color;

  .right-side {
    a {
      margin-left: 20px;
    }
  }

  .left-side {
    a {
      margin-right: 20px;
    }
  }

  img {
    max-width: 650px;
    box-shadow: 0px 0px 10px 10px rgba(0,0,0,0.1);
    transition: 0.25s ease;
    
    &:hover {
      transform: scale(1.005);
      box-shadow: 0px 0px 10px 10px rgba(0,0,0,0.2);
    }
  }

  h2 {
    padding-top: 6rem;
    font-family: 'SF', sans-serif;
    font-size: 2rem;
    margin-bottom: 2rem;
    color: $text-color;
    position: relative;
    padding-bottom: 0.4rem;

    &:after {
    content: "";
    width: 65px;
    height: 4px;
    background-color: $accent-color;
    position: absolute;
    bottom: 0;
    left: 0;
    }
  }

  h3 {
    color: $accent-color;
    font-size: 1.75rem;
    font-family: 'SF', sans-serif;
  }

  a {
    font-family: 'SF', sans-serif;
    text-decoration: none;
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
      justify-content: space-between;
      position: absolute;
      bottom: 0;
      right: 0;
    }

    .right-3d {
      text-align: left;

      h3 {
        text-align: right;
      }

      .portfolio3d-description {
        padding-left: 40px;
        text-align: right;
        padding-top: 20px;
      }

      .portfolio3d-software {
        text-align: right;
        padding-top: 75px;
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

    .weather-description {
      padding-right: 40px;
      padding-top: 20px;
    }

    .weather-software {
      padding-top: 73px;
    }
  }

  #container-frontend {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100%;
    height: 320px;
    position: relative;
    font-family: 'Calibre', sans-serif;
    font-size: 20px;

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

      .frontend-description {
        padding-left: 40px;
        text-align: right;
        padding-top: 20px;
      }

      .frontend-software {
        text-align: right;
        padding-top: 100px;        
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

    .todo-description {
      padding-right: 40px;
      padding-top: 20px;
    }

    .todo-software {
      padding-top: 95px;
    }
  }
}

// Smartphone
@media screen and (max-width: 700px) {
  #projects-container {
  max-width: 100vw;
  padding: 0 2rem;
  font-size: 18px;  

  #projects {
    scroll-margin-top: 50px;
  }

  .right-side {
    a {
      margin-left: 0;
    }
  }

  .left-side {
    a {
      margin-right: 0;
    }
  }

  img {
    width: 100%;
    display: block;
    line-height: 0;
    
    &:hover {
      transform: none;
      box-shadow: 0px 0px 10px 10px rgba(0,0,0,0.1);
    } 
  }

  h2 {
    padding-top: 5rem;
    font-size: 2rem;
    margin-bottom: 2rem;
    padding-bottom: 0.4rem;
  }

  h3 {
    font-size: 20px;
  }

  p {
    font-size: 18px;
    text-align: center;
  }

  a {
    font-family: 'SF', sans-serif;
  }

  .links-buttons {
      text-align: center;
      text-decoration: none;
      justify-content: space-between;
      position: relative;
      display: block;
  }

  #container-3d {
    display: block;
    width: 100%;
    margin-bottom: 225px;

    .image-3d {
      height: 100%;
      text-align: center;
    }

    .links-buttons {
      display: flex;
      position: relative;
    }

    .right-3d {
      text-align: center;

      h3 {
        text-align: center;
        padding-top: 10px;
        width: 100%;
      }

      .portfolio3d-description {
        padding-left: 0;
        text-align: center;
        padding-top: 5px;
        width: 100%;
      }

      .portfolio3d-software {
        text-align: center;
        width: 100%;
        padding-top: 25px;
      }
    }
  }

  #container-weather {
    flex-flow: column-reverse;
    width: 100%;
    margin-bottom: 100px;

    .image-weather {
      text-align: center;
      height: 100%;
    }

    h3 {
      font-size: 20px;
      text-align: center;
      padding-top: 10px;
    }

    .links-buttons {
      position: relative;
      display: flex;
    }

    .weather-description {
      text-align: center;
      width: 100%;
      padding-right: 0;
      padding-top: 5px;
    }

    .weather-software {
      text-align: center;
      padding-top: 25px;
      width: 100%;
    }
  }

  #container-frontend {
    display: block;
    margin-bottom: 200px;
    width: 100%;

    .image-frontend {
      height: 100%;
    }

    .links-buttons {
      display: flex;
      position: relative;
    }

    .right-frontend {
      text-align: center;

      h3 {
        font-size: 20px;
        text-align: center;
        padding-top: 10px;
      }

      .frontend-description {
        padding-left: 0;
        text-align: center;
        padding-top: 5px;
      }

      .frontend-software {
        text-align: center;
        padding-top: 25px;      
      }
    }
  }

  #container-todo {
    margin-bottom: 100px;
    display: flex;
    flex-direction: column-reverse;
    width: 100%;

    .image-todo {
      height: 100%;
    }

    .links-buttons {
      position: relative;
      display: flex;
    }

    h3 {
      font-size: 20px;
      text-align: center;
      color: $accent-color;
      padding-top: 10px
    }

    .todo-description {
      padding-right: 0;
      padding-top: 5px;
    }

    .todo-software {
      padding-top: 25px;
    }
  }
}  
}

// Tablet
@media screen and (min-width: 701px) and (max-width: 1049px){
  #projects-container {
  max-width: 100vw;
  padding: 0 2rem;
  font-size: 18px;  

  #projects {
    scroll-margin-top: 50px;
  }


  img {
    width: 100%;
    line-height: 0;

    &:hover {
      transform: none;
      box-shadow: 0px 0px 10px 10px rgba(0,0,0,0.1);
    } 
  }

  h2 {
    padding-top: 5rem;
    font-size: 3rem;
    margin-bottom: 2rem;
    padding-bottom: 0.4rem;
  }

  h3 {
    font-size: 30px;
  }

  p {
    font-size: 22px;
  }


  #container-3d {
    display: block;
    width: 100%;
    margin-bottom: 500px;


    .image-3d {
      text-align: center;
      height: 100%;
    }

    .links-buttons {
      display: flex;
      position: relative;
      justify-content: center;
      width: 100%;
    }

    .right-3d {
      text-align: center;

      h3 {
        text-align: center;
        padding-top: 10px;
        width: 100%;
      }

      .portfolio3d-description {
        padding-left: 0;
        text-align: center;
        padding-top: 5px;
        width: 90%;
        margin: 0 auto;
      }

      .portfolio3d-software {
        text-align: center;
        width: 100%;
        padding: 25px 0 10px 0;
      }
    }
  }

  #container-weather {
    flex-flow: column-reverse;
    width: 100%;
    margin-bottom: 100px;

    .image-weather {
      text-align: center;
      height: 100%;
    }

    h3 {
      font-size: 20px;
      text-align: center;
      padding-top: 10px;
    }

    .links-buttons {
      position: relative;
      display: flex;
      justify-content: center;
      width: 100%;
    }

    .weather-description {
      text-align: center;
      width: 90%;
      margin: 0 auto;
      padding-right: 0;
      padding-top: 5px;
    }

    .weather-software {
      text-align: center;
      padding-top: 25px;
      width: 100%;
    }
  }

  #container-frontend {
    display: block;
    margin-bottom: 500px;
    width: 100%;

    .image-frontend {
      text-align: center;
      height: 100%;
    }

    .links-buttons {
      display: flex;
      position: relative;
      justify-content: center;
      width: 100%;
    }

    .right-frontend {
      text-align: center;

      h3 {
        font-size: 20px;
        text-align: center;
        padding-top: 10px;
      }

      .frontend-description {
        padding-left: 0;
        text-align: center;
        padding-top: 5px;
        width: 90%;
        margin: 0 auto;
      }

      .frontend-software {
        text-align: center;
        padding-top: 25px;      
      }
    }
  }

  #container-todo {
    margin-bottom: 100px;
    display: flex;
    flex-direction: column-reverse;
    width: 100%;

    .image-todo {
      text-align: center;
      height: 100%;
    }

    .links-buttons {
      width: 100%;
      text-align: center;
      align-items: center;
      position: relative;
      display: flex;
      justify-content: center;
    }

    h3 {
      font-size: 20px;
      text-align: center;
      color: $accent-color;
      padding-top: 10px
    }

    .todo-description {
      padding-right: 0;
      padding-top: 5px;
      width: 90%;
      margin: 0 auto;
      text-align: center;
    }

    .todo-software {
      padding-top: 25px;
      text-align: center;
    }
  }
}  
}
</style>
