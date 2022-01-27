<template>
  <div>
    <FooterMerch/>
    <FooterMap/>
  </div>
</template>

<script>
import FooterMerch from "./FooterMerch.vue";
import FooterMap from "./FooterMap.vue";

export default {
  name: 'Footer',
  components: {
    FooterMerch,
    FooterMap
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
