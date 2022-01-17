<template>
  <footer id="pie">
    <p>© Copyright 2021 - Todos los derechos reservados </p>
    <div id="social">
      <span id="twitter" class="icon"><i class="fab fa-instagram"></i></span>
      <span id="face" class="icon"><i class="fab fa-twitter"></i></span>
      <span id="insta" class="icon"><i class="fab fa-facebook-square"></i></span>
      </div>

  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
#pie {
    background-color: rgb(255, 123, 0);
}
#pie p {
    padding: 2em 0em;
    margin: 0;
    color: white;
    font-weight: bold;
    text-align: center;
    
}
#social{
  padding-bottom: 1em;
}
.icon{
  color: white;
  margin: 0 0.5em;
}
</style>