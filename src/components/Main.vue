<template>
  <section>
    <!-- sezione 1 -->
    <Carousel />
    <!-- sezione 2 -->
    <YourWebsite />
    <!-- sezione 3 -->
    <OurMissions />
    <!-- sezione 4 -->
    <ProjectsMain />
    <!-- sezione 5 -->
    <ArtisticImages />
    <!-- sezione 6 -->
    <JumbotronGuest />
    <!-- sezione 7 -->
    <LatestNews />
    <!-- sezione 8 -->
    <Partnership />
  </section>
</template>

<script>
import Carousel from "../components/Main/Carousel.vue";
import YourWebsite from "../components/Main/YourWebsite.vue";
import OurMissions from "../components/Main/OurMissions.vue";
import ProjectsMain from "../components/Main/ProjectsMain.vue";
import ArtisticImages from "../components/Main/ArtisticImages.vue";
import JumbotronGuest from "../components/Main/JumbotronGuest.vue";
import LatestNews from "../components/Main/LatestNews.vue";
import Partnership from "../components/Main/Partnership.vue";
export default {
  name: "HomeMain",
  components: {
    Carousel,
    YourWebsite,
    OurMissions,
    ProjectsMain,
    ArtisticImages,
    JumbotronGuest,
    LatestNews,
    Partnership,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/main-style.scss";
</style>
