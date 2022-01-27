<template>
  <div class="banner">
    <img src="../assets/img/dc-logo.png" alt="">
    <nav>
      <ul>
        <li v-for="(element,index) in naviItems" :key="index">{{element.text}}</li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return{
      naviItems:[
        {
          text: "Characthers"
          },
        {
          text: "Comics"
        },
        {
          text: "Movies"
        },
        {
          text: "Tv"
        },
        {
          text: "Games"
        },
        {
          text: "Collectibles"
        },
        {
          text: "Videos"
        },
        {
          text: "Fans"
        },
        {
          text: "News"
        },
        {
          text: "Shop"
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";
.banner{
  width: 90%;
  height: 150px;
  padding: 0 100px;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;

  img{
    width: 80px;
  }
}
nav{
  ul{
    list-style: none;
    display: flex;

    li{
      margin: 0px 10px;
      font-weight: bold;
      font-size: 13px;
      text-transform: uppercase;
    }
    li:hover{
      color: $main-color-blue;
      cursor: pointer;
    }
  }
}
</style>
