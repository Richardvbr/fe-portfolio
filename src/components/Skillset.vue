<template>
  <section id="skillset-container" data-aos="fade-up" data-aos-delay="0" data-aos-anchor-placement="top-center">
    <h2 id="skillset">Skill set</h2>
    <p class="description">
      My name is Richard van Brunschot and I am a front-end developer that loves building responsive websites and web apps using the latest technologies.
      <br><br>
    </p>
    <div class="card-skillset">
      <div class="card-skillset__interface">
        <h3>User interface</h3>
        <ul class="interface-list">
          <li class="interface-list__item"></li>
          <li class="interface-list__item"></li>
          <li class="interface-list__item"></li>
          <li class="interface-list__item"></li>
          <li class="interface-list__item"></li>
          <li class="interface-list__item"></li>
          <li class="interface-list__item"></li>
        </ul>
      </div>
      <div class="card-skillset__javascript">
        <h3>JavaScript</h3>
        <ul class="javascript-list">
          <li class="javascript-list__item"></li>
          <li class="javascript-list__item"></li>
          <li class="javascript-list__item"></li>
          <li class="javascript-list__item"></li>
          <li class="javascript-list__item"></li>
          <li class="javascript-list__item"></li>
          <li class="javascript-list__item"></li>
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
$accent-color: #038AFF;


#skillset-container {
  padding-top: 200px;
  max-width: 1050px;
  margin: 0 auto;
  font-family: 'Inter', sans-serif;
  font-size: 17px;
  font-weight: 500;
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
      height: 30rem;
      background-color: #fff;
      box-shadow: 0px 0px 15px 1px rgba(0,0,0,0.2);
      display: flex;
      padding: 1.5rem 3rem 1.5rem 3rem;

      &__javascript {
        margin-left: 30%;
      }
    }
}

@media screen and (max-width: 700px){
  #skillset-container {
    margin-top: 5rem;
    max-width: 100vw;
    padding: 0 2rem;


    .flex-container {
      display: flex;
      flex-direction: column;
      justify-content: center;

      .description{
        text-align: left;
        width: 100%;
        padding-bottom: 10px;
      } 
    }
  } 
}

@media screen and (min-width: 701px) and (max-width: 1049px){
  #skillset-container {
    max-width: 100vw;
    padding: 0 2rem;
    font-size: 22px;
    margin-top: 5rem;

    #skillset {
      scroll-margin-top: -60px;
    }

    .flex-container {
      display: flex;
      flex-direction: column;
      justify-content: center;

      .description{
        text-align: left;
        width: 80%;
        padding-bottom: 10px;
      } 
    }
  } 
}
</style>
