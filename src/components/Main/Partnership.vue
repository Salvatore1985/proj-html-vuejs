<template>
  <section class="bg_primary">
    <div class="container-fluid">
      <div class="row">
        <div class="col-12">
          <!-- card -->
          <CardPartnership :listCard="cardsList" />
        </div>
      </div>
      <div class="col-12 px-3 pb-5">
        <ul class="d-flex justify-content-between" id="my-client">
          <li v-for="(client, index) in listClient" :key="index + 'client'">
            <img
              :src="require(`../../assets/images/${client}.png`)"
              :alt="index"
            />
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
import CardPartnership from "../Main/Partnership/CardPartnership.vue";
export default {
  name: "MainPartnership",
  components: {
    CardPartnership,
  },
  data() {
    return {
      listClient: [
        "client-1-2x",
        "client-9-2x",
        "client-7-2x",
        "client-3-2x",
        "client-4-2x",
        "client-5-2x",
      ],
      cardsList: [
        {
          input: "text",
          bgColor: "black",
          request: "are you ready?",
          text: "strat a new project",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
        {
          input: "button",
          bgColor: "green",
          request: "what are you waiting for?",
          text: "let's talk about work",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@import "../../components/style/main-style.scss";

.row {
  height: $partenership;
}
#my-client {
  padding-bottom: 3.5rem;
}
</style>

