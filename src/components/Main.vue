<template>
  <div class="main ">
    <div class="container">
      <span> *Content goes here* </span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main{
  background-color: rgba(0, 0, 0, 0.884);
  height: 200px;

  &>div{
    height: 100%;
    display: flex;
    align-items: center;

    span{
    color: white;
    font-size: 30px;
    font-weight: bold;
    }
  }

  
}
</style>
