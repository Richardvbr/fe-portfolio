<template>
  <section id="projects-container" data-aos="fade-up" data-aos-delay="0">
    <h2 id="projects">Projects</h2>
    <div class="grid-container" >
      <!-- Loop over JSON object containing all project data and render a card for each entry -->
      <div class="grid-item" v-for="(project, portfolioLoop) in portfolioJSON" :key="portfolioLoop">
        <div>
          <a :href="project.url" target="_blank"><img :src="project.img" :alt="project.imgAlt"></a>
        </div>
        <div>
          <a :href="project.url" target="_blank"><h3>{{ project.title }}</h3></a>
        </div>
        <!-- Loop over software, creating a tag for each entry (nested loop) -->
        <div class="software">
          <p v-for="(software, softwareLoop) in project.software" :key="softwareLoop">
           {{ software }}
          </p>
        </div>
        <div>
          <p>{{ project.description }}</p>
          <br>
          <p class="project-note">{{ project.note }}</p>
        </div>
        <div class="flex-icons">
          <div class="item1"><a :href="project.github" target="_blank"><i class="fab fa-github"></i></a></div>
          <div class="item2"><a :href="project.url" target="_blank"><i class="fas fa-external-link-alt"></i></a></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Projects',
  data: function () {
    return  {
      portfolioJSON: [
        {
          img: require("../assets/hero_netflix.jpg"),
          imgAlt: 'Netflix React App',
          url: 'https://netflix-react-app-fd806.web.app/',
          title: 'Netlix React App',
          software: ['React.js', 'Firebase', 'Axios', 'CSS'],
          description: "Netflix UI clone built with React.js (including Redux and React Router). Fetches data from TMDB API. Single-page, component-based application. Drag-to-scroll poster rows.",
          note: "Work in progress: authentication (sign-up, sign-in/out) using Firebase.",
          github: 'https://github.com/Richardvbr/netflix-react-app'
        },
        {
          img: require("../assets/hero_3d.jpg"),
          imgAlt: '3D Modeling Portfolio',
          url: 'https://richardvbr-3d-vue.netlify.app/',
          title: '3D Modeling Portfolio',
          software: ['Vue.js', 'SCSS', 'AdobeXD'],
          description: "Portfolio website to showcase 3D models. Component-based Vue.js single-page application to provide a performant and modern experience. New portfolio items are added to the grid automatically using JSON and for-loops.",
          github: 'https://github.com/Richardvbr/3d-portfolio-vue'
        },
        {
          img: require("../assets/hero_weather.jpg"),
          imgAlt: 'Weather App',
          url: 'https://todays-weather-rvbr.herokuapp.com/',
          title: 'Weather App',
          software: ['JavaScript', 'HTML5', 'SCSS', 'AdobeXD'],
          description: "Weather application that displays local current weather information. Fetches weather data using the Dark Sky API. API calls are done on a Node/Express back-end so that the API key is hidden and secured.",
          note: "Note: may take a moment to load due to free Node.js hosting",
          github: 'https://github.com/Richardvbr/Todaysweather'
        },
        {
          img: require("../assets/hero_fe.jpg"),
          imgAlt: 'Front-end Portfolio',
          url: 'https://www.brunschot.dev/',
          title: 'Front-end Portfolio',
          software: ['Vue.js', 'HTML5', 'SCSS', 'AdobeXD'],
          description: "Portfolio website to showcase my work as a front-end developer. Component-based Vue.js application. New portfolio items are added to the grid automatically using JSON and for-loops. Opted for a clean design that is easy on the eyes. Responsive design and scroll-based animations.",
          github: 'https://github.com/Richardvbr/fe-portfolio'
        },
        {
          img: require("../assets/hero_landing.jpg"),
          imgAlt: 'Landing Page',
          url: 'https://richardvbr-landing-page.netlify.app/',
          title: 'Landing Page',
          software: ['HTML5', 'SCSS', 'JavaScript'],
          description: "Fully responsive landing page based on an existing design. Coded using a mobile-first approach. Reponsive navbar that toggles between the default view and a hamburger menu based on device width. Toggleable features using JavaScript.",
          github: 'https://github.com/Richardvbr/Landing-page'
        },
        {
          img: require("../assets/hero_vue_todo.jpg"),
          imgAlt: 'Vue 3 To-do App',
          url: 'https://richardvbr-vue3-todo.netlify.app/',
          title: 'Vue 3 To-do App',
          software: ['Vue 3', 'JavaScript', 'SCSS'],
          description: "A to-do application, made with Vue 3 to try out the new composition API. Stores to-do items in the browser's localStorage. Easily check/uncheck items. Also created a version with vanilla JavaScript to see how it differs from using a framework.",
          github: 'https://github.com/Richardvbr/Vue-3-To-do-Application'
        },
        {
          img: require("../assets/hero_todo.jpg"),
          imgAlt: 'To-do App',
          url: 'https://richardvbr-todoapp.netlify.app/',
          title: 'To-do App',
          software: ['JavaScript', 'HTML5', 'CSS'],
          description: "To-do application that uses the browser's localStorage to store to-do items. Shows current date and prevents empty inputs.",
          github: 'https://github.com/Richardvbr/Todo-app'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #333;
$accent-color: #3da361;
$softwareBGColor: #c3e7cf;

#projects-container {
  max-width: 1150px;
  position: relative;
  margin: 0 auto;
  font-family: 'Inter', sans-serif;
  font-size: 17px;  
  font-weight: 500;
  color: $text-color;

  h2 {
    padding-top: 6rem;
    font-family: 'Inter', sans-serif;
    font-size: 2rem;
    margin-bottom: 3rem;
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

  .grid-container {
    max-width: 100%;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 2.5rem;

    .grid-item {
      width: 100%;
      height: 37.5rem;
      background-color: #fff;
      box-shadow: 0px 0px 15px 1px rgba(0,0,0,0.2);
      position: relative;
      transition: 0.2s ease;
      border-radius: 5px;

      &:hover {
        box-shadow: 0px 0px 15px 1px rgba(0,0,0,0.4);
      }

      img {
        border-radius: 5px 5px 0 0;
        width: 100%;
        display: block;
        border: none;
        clip-path: polygon(0 0, 100% 0, 100% 89%, 0% 100%);
      }

      a {
        color: $text-color;
        text-decoration: none;
      }

      h3 {
        padding: 0 1.5rem;
        font-size: 1.6rem;
        font-weight: bold;
        margin-top: 1.2rem;
      }

      .software {
        display: flex;
        padding: 0 1.5rem;

        p {
          margin: 0.5rem 0.5rem 0.5rem 0;
          padding: 0.3rem;
          border-radius: 5px;
          margin-bottom: 2rem;
          font-size: 12px;
          background-color: $softwareBGColor;
        }
      }

      .project-note {
        font-weight: bold;
        font-size: 14px;
        font-style: italic;
      }

      p {
        padding: 0 1.5rem;
        color: #555;
        line-height: 1.5;
      }

      .flex-icons {
        display: flex;

        .item1 {
          position: absolute;
          bottom: 1.5rem;
          right: 4.25rem;
        }

        .item2 {
          position: absolute;
          bottom: 1.5rem;
          right: 1.5rem;
        }

        i {
          font-size: 27px;
          color: #444;
          transition: 0.2s ease;

          &:hover {
            color: $accent-color;
          }
        }
      }
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

  .grid-container {
    grid-template-columns: 1fr;

    p {
      text-align: left;
    }

    .grid-item {
      box-shadow: 0px 0px 15px 1px rgba(0,0,0,0.1);

      &:hover {
        transform: none;
      }
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

  .grid-container {
    grid-template-columns: repeat(2, 1fr);
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
    font-size: 18px;
  }
}  
}
</style>
