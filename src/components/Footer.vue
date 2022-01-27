<template>
  <div>
    <FooterMerch/>
    <FooterMap/>
    <FooterSocial/>
  </div>
</template>

<script>
import FooterMerch from "./FooterMerch.vue";
import FooterMap from "./FooterMap.vue";
import FooterSocial from "./FooterSocial.vue";

export default {
  name: 'Footer',
  components: {
    FooterMerch,
    FooterMap,
    FooterSocial
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
