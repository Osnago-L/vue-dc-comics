<template>
  <div class="blue-footer">   
      <div class="container">
        <div v-for="(element,index) in merchItems" :key="index" class="merch-item">
          <img :src="element.img" alt="">
          <span>{{element.text}}</span>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Merch",
    data() {
    return{
      merchItems:[
          {
          text: "Digital Comics",
          img: require("../assets/img/buy-comics-digital-comics.png")
          },
          {
          text: "DC Merchandise",
          img: require("../assets/img/buy-comics-merchandise.png")
          },
          {
          text: "Subscription",
          img: require("../assets/img/buy-comics-subscriptions.png")
          },
          {
          text: "Comic Shop Locator",
          img: require("../assets/img/buy-comics-shop-locator.png")
          },
          {
          text: "DC Power Visa",
          img: require("../assets/img/buy-dc-power-visa.svg")
          },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";
.blue-footer{
  height: 200px;
  background-color: $main-color-blue;

  &>div{
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
}
.merch-item{
  display: flex;
  align-items: center;
  
  img{
    width: 45px;
    height: 57px;
    margin-right: 15px;
  }
  span{
    color: white;
    text-transform: uppercase;
  }
}

</style>

