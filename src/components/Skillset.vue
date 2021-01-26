<template>
  <section id="skillset-container" data-aos="fade-up" data-aos-delay="0" data-aos-anchor-placement="top-center">
    <h2 id="skillset">Skill set</h2>
    <p class="description">
      My name is Richard van Brunschot and I am a front-end developer who loves building responsive websites and web apps using the latest technologies.
      <br><br>
    </p>
    <div class="card-skillset">
      <div class="card-skillset__interface">
        <h3>User interface and tools</h3>
        <ul class="interface-list">
          <li class="interface-list__item">HTML5, CSS3, SCSS</li>
          <li class="interface-list__item">Experience with responsive and mobile-first design</li>
          <li class="interface-list__item">Basic UX/UI skills, good eye for detail</li>
          <li class="interface-list__item">Experience with Bootstrap 5</li>
          <li class="interface-list__item">Basic understanding of Tailwind CSS</li>
          <li class="interface-list__item">Familiar with SEO principles</li>
          <li class="interface-list__item">VS Code, Git, Adobe Suite, Wordpress</li>
          <li class="interface-list__item">Unreal Engine 4, Unity</li>
        </ul>
      </div>
      <div class="card-skillset__javascript">
        <h3>JavaScript</h3>
        <ul class="javascript-list">
          <li class="javascript-list__item">JavaScript ES6+</li>
          <li class="javascript-list__item">Experience with Vue.js and React.js</li>
          <li class="javascript-list__item">Displaying data fetched from an API</li>
          <li class="javascript-list__item">Creating single-page applications</li>
          <li class="javascript-list__item">Familiar with npm, webpack, eslint</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'skillset'
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #555;
// $accent-color: #038AFF;
$accent-color: #3da361;


#skillset-container {
  padding-top: 200px;
  max-width: 1150px;
  margin: 0 auto;
  font-family: 'Inter', sans-serif;
  font-size: 16px;
  font-weight: 400;
  color: $text-color;

  h2 {
    font-size: 2rem;
    margin-bottom: 3rem;
    color: #333;
    position: relative;
    padding-bottom: 0.4rem;
    font-family: 'Inter', sans-serif;

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

  .description{
    width: 550px;
    padding-bottom: 10px;
  }

  .card-skillset {
    width: 75%;
    height: 25rem;
    background-color: #fff;
    box-shadow: 0px 0px 15px 1px rgba(0,0,0,0.2);
    display: flex;
    padding: 1.5rem 3rem 1.5rem 3rem;

    &__interface {
      width: 40ch;
    }

    ul {
    padding: 0 2rem;
    list-style: square;

      li {
        margin: 1rem 0;
      }
    }
  }
}

@media screen and (max-width: 700px){
  #skillset-container {
    padding-top: 200px;
    max-width: 1050px;
    margin: 0 2rem;
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    font-weight: 400;
    color: $text-color;

    .description{
      width: 100%;
      padding-bottom: 10px;
    }

    .card-skillset {
      width: 100%;
      height: 48rem;
      display: flex;
      flex-direction: column;
      padding: 1.5rem 2rem 1.5rem 2rem;

      &__interface {
        width: 100%;
      }

      h3 {
        font-weight: bold;
        font-size: 1.25rem;
      }

      ul {
      padding: 0 1rem;
      list-style: square;

        li {
          margin: 1rem 0;
        }
      }
    }
  }
}


@media screen and (min-width: 701px) and (max-width: 1049px){
  #skillset-container {
    padding-top: 200px;
    max-width: 1050px;
    margin: 0 2rem;
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    font-weight: 400;
    color: $text-color;

    .description{
      width: 100%;
      padding-bottom: 10px;
    }

    .card-skillset {
      width: 100%;
      height: 30rem;
      display: flex;
      padding: 1.5rem 2rem 1.5rem 2rem;

      &__interface {
        width: 35ch;
      }

      h3 {
        font-weight: bold;
        font-size: 1.25rem;
      }

      ul {
      padding: 0 1rem;
      list-style: square;
      font-size: 1.1rem;

        li {
          margin: 1rem 0;
        }
      }
    }
  }
}
</style>
