<template>
  <div class="container">
    <div class="footer">
      <p>Design &amp; Code by Richard van Brunschot</p>
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
    color: $text-color;
    height: 100%;
    font-size: 15px;
    box-shadow: 0px -10px 15px 1px rgba(0,0,0,0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 5px;
  }
}
</style>
