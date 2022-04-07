<template>
  <div>
    <HeaderSocial />
    <HeaderNav />
  </div>
</template>

<script>
import HeaderSocial from "../components/Header/HeaderSocial.vue";
import HeaderNav from "../components/Header/HeaderNav.vue";
export default {
  name: "HomeHeader",
  components: {
    HeaderSocial,
    HeaderNav,
  },
  data() {
    return {};
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
