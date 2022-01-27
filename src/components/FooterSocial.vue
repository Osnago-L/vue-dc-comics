<template>
  <div class="social">   
    <div class="container">
      <button>SIGN UP NOW!</button>
      <div class="social-icons">
        <span>FOLLOW</span>
        <div><img v-for="element,index in icons" :key="index" :src="element.img" alt=""> </div>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
    name:"FooterSocial",
    data() {
    return{
      icons:[
          {
          text: "Facebook",
          img: require("../assets/img/footer-facebook.png")
          },
          {
          text: "Twitter",
          img: require("../assets/img/footer-twitter.png")
          },
          {
          text: "YouTube",
          img: require("../assets/img/footer-youtube.png")
          },
          {
          text: "Pinterest",
          img: require("../assets/img/footer-pinterest.png")
          },
          {
          text: "Periscope",
          img: require("../assets/img/footer-periscope.png")
          },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import "../assets/style/partials/variables.scss";
.social{
  height: 60px;
  background-color: rgba(0, 0, 0, 0.85);

  &>div{
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  button{
    background: none;
    color: inherit;
    border: 1px solid $main-color-blue;
    padding: 10px;
    cursor: pointer;
    color: white;
  }
  
  .social-icons{
    display: flex;
    align-items: center;
    gap: 10px;
    
    span{
    color: $main-color-blue;
    }
    img{
      margin: 0 6px ;
    }
  }
}
</style>

