<template>
  <div class="container">
    <div class="footer">
      <a href="https://github.com/Richardvbr" target="_blank">Design &amp; Code by Richard van Brunschot</a>
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
    font-family: 'Inter', sans-serif;
    background-color: #fff;
    height: 100%;
    font-size: 15px;
    box-shadow: 0px -10px 15px 1px rgba(0,0,0,0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 7px;
    font-weight: 500;

    a {
      color: rgb(90, 90, 90);
      text-decoration: none;
    }
  }
}
</style>
