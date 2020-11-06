<template>
  <section id="about-container" data-aos="fade-up" data-aos-delay="0" data-aos-anchor-placement="top-center">
    <div class="flex-container">
      <h2 id="about">About Me</h2>
      <p class="description">
        Hi, my name is Richard and I'm a front-end developer based in Veldhoven, The Netherlands. <br> <br> I enjoy creating things that live on the internet, whether that be websites, applications, or anything in between. I aim to build responsive products that provide performant experiences and are easy to use. <br> <br>
        Here are a few technologies I've been working with recently:
      </p>
      <ul class="software">
        <li><i class="fas fa-caret-right"></i>JavaScript (ES6+)</li>
        <li><i class="fas fa-caret-right"></i>Vue.js</li>
        <li><i class="fas fa-caret-right"></i>Vue Router</li>
        <li><i class="fas fa-caret-right"></i>PHP</li>
        <li><i class="fas fa-caret-right"></i>WordPress</li>
        <li><i class="fas fa-caret-right"></i>HTML5</li>
        <li><i class="fas fa-caret-right"></i>(S)CSS</li>
        <li><i class="fas fa-caret-right"></i>AdobeXD</li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #555;
$accent-color: #038AFF;


#about-container {
  padding-top: 200px;
  max-width: 1050px;
  margin: 0 auto;
  font-family: 'Inter', sans-serif;
  font-size: 17px;
  font-weight: 500;
  color: $text-color;

  .flex-container {
    display: flex;
    // height: 100%;
    flex-direction: column;
    justify-content: center;

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

    ul {
      columns: 2;
      width: 550px;
      list-style: none;
      font-size: 16px;


      i {
        color: $accent-color;
        padding: 10px 10px 0 0;
      }
    }
  }
}

@media screen and (max-width: 700px){

 #about-container {
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

    ul {
      width: 100%;
      font-size: 15px;

      i {
        padding: 10px 10px 0 0;
      }
    }
  }
} 
}

@media screen and (min-width: 701px) and (max-width: 1049px){
 #about-container {
  max-width: 100vw;
  padding: 0 2rem;
  font-size: 22px;
  margin-top: 5rem;

  #about {
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

    ul {
      width: 100%;

      i {
        padding: 10px 10px 0 0;
      }
    }
  }
} 
}
</style>
