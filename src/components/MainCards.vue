<template>
  <div class="cards">
      <img :src="cardsData.thumb" alt="">
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
    width: 200px;
    display: flex;
    flex-direction: column;

    img{
        object-position: 0px 0px;
        object-fit: cover;
        width: 100%;
        height: 230px;
    }

    span{
        margin-top: 15px;
        color: white;
        font-size: 15px;
    }
}
</style>