<template>
  <section class="">
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-7">
          <div class="container-fluid">
            <div class="row my-card">
              <div class="col-12 d-flex justify-content-center">
                <!-- card -->
                <CardPartnership class="bg-black" :listCard="cardsList" />
              </div>
            </div>
          </div>
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
          request: "are you ready?",
          text: "strat a new project",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
        {
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
.col-5 {
  height: $you_web_height;
  z-index: 1;
  div {
    h1 {
      font-size: 3.8rem;
    }
    h5 {
      color: #00d9a6;
    }
  }
}
.my-card {
  height: $you_web_height;
}
</style>

