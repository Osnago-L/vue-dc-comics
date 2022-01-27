<template>
  <div class="banner">
    <img src="../assets/img/dc-logo.png" alt="">
    <nav>
      <ul>
        <li></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.banner{
  width: 90%;
  height: 150px;
  padding: 0 100px;
  border: 1px solid black;
  margin: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;

  img{
    width: 100px;
  }
}
nav{
  display: flex;
}
</style>
