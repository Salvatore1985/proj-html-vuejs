<template>
  <footer>
    <FooterNav />
    <FooterSocial />
  </footer>
</template>

<script>
import FooterNav from "./Footer/FooterNav.vue";
import FooterSocial from "./Footer/FooterSocial.vue";
export default {
  name: "HomeFooter",
  components: {
    FooterNav,
    FooterSocial,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
