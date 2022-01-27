<template>
  <div class="map">
      <div class="container"></div>
  </div>
</template>

<script>
export default {
    name:"Map",
    data() {
    return{
      navItems:[
          {
          text: "Digital Comics",
          img: "../assets/img/buy-comics-digital-comics.png"
          },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";
.map{
  background-image: url("../assets/img/footer-bg.jpg");
  height: 500px;
  background-position: cover;
  background-size: 100vw 500px;
}
</style>

