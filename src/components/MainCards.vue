<template>
  <div class="cards">
      <div class="cardimage"></div>
      <span>{{cardsData.series}}</span>
  </div>
</template>

<script>
export default {
    name: "MainCards",
    props:{
        cardsData: Object
    }
}
</script>

<style lang="scss" scoped>
.cards{
    width: 120px;
    display: flex;
    flex-direction: column;

    .cardimage{
        background-image: url("https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX");
        background-position: center;
        background-position-y: 0px;
        background-size: cover;
        width: 100%;
        height: 130px;
        
    }
    span{
        margin-top: 5px;
        color: white;
        font-size: 13px;
    }
}
</style>