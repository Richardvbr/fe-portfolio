<template>
  <div class="container">
    <div class="footer">
      <a href="https://github.com/Richardvbr">Design &amp; Code by Richard van Brunschot</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped lang="scss">
// Variables
$text-color: #333;

.container {
  height: 3rem;

  .footer {
    font-family: 'Calibre', sans-serif;
    background-color: #fff;
    height: 100%;
    font-size: 15px;
    box-shadow: 0px -10px 15px 1px rgba(0,0,0,0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 5px;

    a {
      color: $text-color;
      text-decoration: none;
    }
  }
}
</style>
