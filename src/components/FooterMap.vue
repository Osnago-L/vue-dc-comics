<template>
  <div class="map">
      <div class="container">
        <div class="map-list">
          <ul v-for="ul,indexUL in mapCategories " :key="indexUL">{{ul.text}}
            <li v-for="li,indexLI in mapCategories[indexUL].content " :key="indexLI">{{li.text}}</li>
          </ul>
        </div>
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
  </div>
</template>

<script>
export default {
    name:"FooterMap",
    data() {
    return{
      mapCategories:[
          {
          text: "DC Comics",
          content:[
            {
              text: "Elemento1"
            },
            {
              text: "Elemento2"
            },
            {
              text: "Elemento3"
            },
            {
              text: "Elemento4"
            },
            {
              text: "Elemento5"
            },
          ]
          },
          {
          text: "Shop",
          content:[
            {
              text: "Elemento6"
            },
            {
              text: "Elemento7"
            },
          ]
          },
          {
          text: "DC",
          content:[
            {
              text: "Elemento12"
            },
            {
              text: "Elemento13"
            },
            {
              text: "Elemento14"
            },
            {
              text: "Elemento15"
            },
            {
              text: "Elemento16"
            },
            {
              text: "Elemento171"
            },
            {
              text: "Elemento171"
            },
            {
              text: "Elemento171"
            },
            {
              text: "Elemento171"
            },

          ]
          },
          {
          text: "Sites",
          content:[
            {
              text: "Elemento18"
            },
            {
              text: "Elemento19"
            },
            {
              text: "Elemento20"
            },
            {
              text: "Elemento21"
            },
            {
              text: "Elemento22"
            },
            {
              text: "Elemento23"
            },

          ]
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
  height: 380px;
  background-position: cover;
  background-size: 100vw 400px;
  padding: 30px 0;
  overflow-y: hidden;
  

  &>div{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    img{
      width:600px;
      height: 600px;
    }
  }
}
.map-list{
  width: 500px;
  height: 100%;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;

  ul{
    margin-bottom: 15px;
    list-style: none;
    color: white;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 20px;
    cursor: pointer;
    
    li{
      color: grey;
      text-transform: capitalize;
      font-weight: normal;
      font-size: 14px;
      margin: 10px 0;
      cursor: pointer;
    }
  }
}
</style>

