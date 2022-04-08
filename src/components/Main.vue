<template>
  <section>
    <Carousel />
    <YourWebsite />
    <OurMissions />
    <ProjectsMain />
    <ArtisticImages />
    <JumbotronGuest />
  </section>
</template>

<script>
import Carousel from "../components/Main/Carousel.vue";
import YourWebsite from "../components/Main/YourWebsite.vue";
import OurMissions from "../components/Main/OurMissions.vue";
import ProjectsMain from "../components/Main/ProjectsMain.vue";
import ArtisticImages from "../components/Main/ArtisticImages.vue";
import JumbotronGuest from "../components/Main/JumbotronGuest.vue";
export default {
  name: "HomeMain",
  components: {
    Carousel,
    YourWebsite,
    OurMissions,
    ProjectsMain,
    ArtisticImages,
    JumbotronGuest,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
