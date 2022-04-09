<template>
  <section class="bg_primary">
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <!-- card -->
          <CardPartnership :listCard="cardsList" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import CardPartnership from "./CardPartnership.vue";
export default {
  name: "MainPartnership",
  components: {
    CardPartnership,
  },
  data() {
    return {
      cardsList: [
        {
          bgColor: "black",
          request: "are you ready?",
          text: "strat a new project",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
        {
          bgColor: "green",
          request: "what are you waiting for?",
          text: "let's talk about work",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
      ],
    };
  },
  methods: {
    changeImg(index) {
      /* console.log(this.groupList[index].id); */
      if (this.groupList[index].id == "01") {
        console.log("primo");
      } else if (this.groupList[index].id == "02") {
        console.log("secondo");
      } else {
        console.log("terzo");
      }
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/components/style/main-style.scss";

.row {
  height: $partenership;
}
</style>

