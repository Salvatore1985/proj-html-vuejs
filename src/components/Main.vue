<template>
  <section>
    <Carousel />
    <YourWebsite />
    <OurMissions />
  </section>
</template>

<script>
import Carousel from "../components/Main/Carousel.vue";
import YourWebsite from "../components/Main/YourWebsite.vue";
import OurMissions from "../components/Main/OurMissions.vue";
export default {
  name: "HomeMain",
  components: {
    Carousel,
    YourWebsite,
    OurMissions,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
