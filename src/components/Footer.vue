<template>
  <footer class="container">
    <div class="footer">
      <a href="https://github.com/Richardvbr" target="_blank">Design &amp; Code by Richard van Brunschot</a>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped lang="scss">
// Variables
$text-color: #333;
$accent-color: #3da361;

.container {
  height: 3rem;

  .footer {
    font-family: 'Inter', sans-serif;
    background-color: #fff;
    height: 100%;
    font-size: 13px;
    box-shadow: 0px -10px 15px 1px rgba(0,0,0,0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: 500;

    a {
      color: rgb(90, 90, 90);
      text-decoration: none;
      transition: .2s ease;

      &:hover {
        color: $accent-color;
      }
    }
  }
}

@media screen and (max-width: 700px) {
  .container .footer a {
    font-size: 13px;
  }
}
</style>
