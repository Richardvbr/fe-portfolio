<template>
  <section id="contact-container" data-aos="fade-up" data-aos-delay="0" data-aos-anchor-placement="top-center">
    <h2 id="contact">Contact</h2>
    <div class="flex-container">
      <div class="left">
        <p class="description">Feel free to contact me by using the contact form. Alternatively, you can reach me by using the options below.</p>
        <h3>Email</h3>
        <a href="mailto:richardvanbrunschot@gmail.com">Richardvanbrunschot@gmail.com</a>
        <div class="link-buttons">
          <a href="https://www.linkedin.com/in/rbrunschot/" target=”_blank” rel=”noreferrer“><button class="button-link">LinkedIn <i class="fas fa-external-link-alt"></i></button></a>
          <a href="https://github.com/Richardvbr" target="_blank"><button class="button-link">GitHub <i class="fas fa-external-link-alt"></i></button></a>
        </div>
      </div>
      <div class="right">
        <form name='contact' method='POST' action="https://submit-form.com/Otq_rxofDoDfHq6iSLaem"><input type='hidden' name='form-name' value='contact' />
          <p>
            <label>Name</label>
            <input type="text" name="name" required>
          </p>
          <p>
            <label>Email</label>
            <input type="email" name="email" required>
          </p>
          <p class="full">
            <label>Message</label>
            <textarea name="message" rows="5" required></textarea>
          </p>
          <div class="full submit-button">
            <button type="submit">Submit</button>
          </div>
        </form>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Contact'
}
</script>

<style scoped lang="scss">
// Variables
$background-color: #f7f7f7;
$text-color: #555;
$accent-color: #4d6bd8;
$border-color: #b4b4b4;

#contact-container {
  padding: 300px 0;
  max-width: 1050px;
  // height: 100vh;
  position: relative;
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

  .flex-container {
    display: flex;
    height: 100%;
    flex-direction: row;

    .left {
      max-width: 350px;
      padding-top: 20px;
      margin-right: 50px;

      h3 {
        font-family: 'Inter', sans-serif;
        color: $accent-color;
        padding-top: 30px;
        font-size: 20px;
      }

      a {
        text-decoration: none;
        color: $text-color;
        margin-right: 20px;
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
        font-family: 'Inter', sans-serif;
        transition: 0.25s ease;
        margin-top: 27px;

        &:hover {
          color: $background-color;
          background-color: $accent-color;
        }

        i {
          margin-left: 10px;
        }
      }
    }

    form {
      display: grid;
      grid-template-columns: 1fr 1fr;
      grid-gap: 15px;
    }

    .full {
      grid-column: 1 / 3;
    }

    .submit-button {
      button {
      width: 50%;
      padding: 0.75rem 2.5rem;
      font-size: 18px;
      background: none;
      border: 2px solid $accent-color;
      border-radius: 13px;
      font-family: 'Inter', sans-serif;
      text-align: center;
      cursor: pointer;
      color: $accent-color;
      transition: 0.25s ease;
      margin-left: 25%;
      margin-top: 25px;
      font-weight: 600;

        &:hover {
          background-color: $accent-color;
          color: $background-color;
        }
      }
    }

    label {
      display: block;
      font-size: 17px;
    }

    input {
      background: none;
      border: 1px solid $border-color;
      border-radius: 3px;
      padding: 0.5rem;
      font-family: 'Inter', sans-serif;
      font-size: 17px;
      color: #555;
      font-weight: 500;

      &:focus {
      border: 1px solid $accent-color;
      outline: 0 none;
      }

      &:focus-within label {
        color: red;
      }
    }

    textarea {
      font-family: 'Inter', sans-serif;
      background: none;
      resize: none;
      width: 100%;
      border: 1px solid $border-color;
      border-radius: 3px;
      font-size: 20px;
      padding-left: 0.5rem;
      padding-top: 0.5rem;
      margin-top: 0.2rem;
      font-size: 17px;
      color: #555;
      font-weight: 500;

      &:focus {
        border: 1px solid $accent-color;
        outline: 0 none;
      }
    }
  }
}

// Smartphone
@media screen and (max-width: 700px) {

 #contact-container {
  padding: 100px 2rem 5rem 2rem;
  max-width: 100vw;

  #contact {
    scroll-margin-top: 200px;
  }

  .flex-container {
    display: flex;
    flex-direction: column-reverse;

    .left {
      max-width: 375px;
      padding-top: 20px;

      h3 {
        font-family: 'Inter', sans-serif;
        color: $accent-color;
        padding-top: 30px;
        font-size: 20px;
      }

      a {
        text-decoration: none;
        color: $text-color;
        margin-right: 20px;
      }
    }

    form {
      grid-template-columns: 1fr;
    }

    .submit-button {
      button {
        width: 60%;
        margin: 15px 0;
      }
    }

    .full {
      grid-column: 1;
    }
  }
} 
}

// Tablet
@media screen and (min-width: 701px) and (max-width: 1049px) {
 #contact-container {
  padding: 100px 2rem 5rem 2rem;
  max-width: 100vw;

  #contact {
    scroll-margin-top: -75px;
  }

  .flex-container {
    display: flex;
    flex-direction: column-reverse;

    .left {
      max-width: 375px;
      padding-top: 20px;

      h3 {
        font-family: 'Inter', sans-serif;
        color: $accent-color;
        padding-top: 30px;
        font-size: 20px;
      }

      a {
        text-decoration: none;
        color: $text-color;
        margin-right: 20px;
      }
    }

    form {
      grid-template-columns: 1fr;
    }

    .submit-button {
      button {
      width: 25%;
      margin-left: 0;
      margin: 15px 0;
      }
    }

    .full {
      grid-column: 1;
    }

    textarea {
      width: 50%;
    }
  }
} 
}
</style>
