<template>
  <section class="bg_primary">
    <h2 class="text-center">lastest news & our <span>blog</span></h2>
    <div class="d-flex justify-content-center">
      <Decoration class="py-3" />
    </div>
    <div>
      <LatestNewsCard :listCard="laterstCardList" />
    </div>
  </section>
</template>

<script>
import Decoration from "../ComponentsDecoration/Decoration.vue";
import LatestNewsCard from "../Main/LatestNewsCard.vue";
export default {
  nome: "LatestNews",
  components: {
    Decoration,
    LatestNewsCard,
  },
  data() {
    return {
      laterstCardList: [
        {
          src: "serious-businesswoman-with-documents-talking-on-P9Q6LX6-1024.jpg",
          date: "may 24, 2018 .by Alex",
          new: "marketing ideas",
          id: "01",
        },
        {
          src: "Businessman-at-the-desk-in-his-office-resting--1024x768.jpg",
          date: "may 24, 2018 .by Alex",
          new: "rest during working hours",
          id: "02",
        },
        {
          src: "simple-home-office-with-tree-PBXRXYB-large-1024x768.jpg",
          date: "may 24, 2018 .by Alex",
          new: "develop your startup idea",
          id: "03",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
section {
  /*   height: 1000px; */
  h2 {
    padding: 15rem 0 4rem 0;
    font-size: 3.5rem;
    span {
      color: #00d9a6;
    }
  }
}
</style>