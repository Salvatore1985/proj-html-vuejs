<template>
  <section>
    <div class="cover-carousel" v-for="cover in listSlide" :key="cover.id">
      <img :src="require(`@/assets/images/${cover.url}`)" :alt="cover.text" />
    </div>
  </section>
</template>

<script>
export default {
  name: "SlideCarousel",
  props: ["visibleCover", "listSlide"],
  components: {},
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@import "../../components/style/main-style.scss";

.cover-carousel {
  height: $carousel_height;
  width: 100%;

  overflow: hidden;
  position: relative;

  img {
    width: 1200px;
    height: $carousel_height;
    object-fit: cover;
    object-position: center;
    object-position: right;
    position: absolute;
  }
}
</style>

