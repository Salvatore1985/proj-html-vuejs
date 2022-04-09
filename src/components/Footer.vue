<template>
  <footer>
    <FooterNav />
  </footer>
</template>

<script>
import FooterNav from "./Footer/FooterNav.vue";
export default {
  name: "HomeFooter",
  components: {
    FooterNav,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
