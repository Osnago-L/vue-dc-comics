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
          img: "../../../assets/img/buy-comics-digital-comics.png"
          },
          {
          text: "Digital Comics",
          img: "../../../assets/img/buy-comics-digital-comics.png"
          },
          {
          text: "Digital Comics",
          img: "../../../assets/img/buy-comics-digital-comics.png"
          },
          {
          text: "Digital Comics",
          img: "../../../assets/img/buy-comics-digital-comics.png"
          },
          {
          text: "Digital Comics",
          img: "../../../assets/img/buy-comics-digital-comics.png"
          },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../../../assets/style/partials/variables.scss";
.blue-footer{
  height: 200px;
  background-color: $main-color-blue;

  &>div{
    height: 100%;
    display: flex;
    align-items: center;
  }
}
.merch-item{
  display: flex;

  img{
    width: 200px;
    margin-right: 15px;
  }
}

</style>

