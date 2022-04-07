<template>
  <section>
    <Carousel />
  </section>
</template>

<script>
import Carousel from "../components/Main/Carousel.vue";
export default {
  name: "HomeMain",
  components: {
    Carousel,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
