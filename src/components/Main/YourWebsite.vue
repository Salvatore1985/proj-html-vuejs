<template>
  <section class="bg_primary">
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-5 ps-5 py-5">
          <div>
            <h1 class="py-3">
              We Are a Here To Marke Your
              <span class="text_color_color_primary">Website</span>
              Look More
              <span class="text_color_color_primary">Elegant</span>
              And Stulish!
            </h1>
          </div>
          <!-- Aggiunto componente style  -->
          <Decoration class="py-3" />
          <div class="py-4">
            <button class="rounded-pill border-0 green" type="submit">
              read more
            </button>
          </div>
          <!-- Cards -->
          <div
            class="py-5 d-flex justify-content-between align-items-center"
          ></div>
        </div>
        <div class="col-7">
          <div class="container">
            <div class="row">
              <div class="col-6">
                <Card />
              </div>
              <div class="col-6">
                <Card />
              </div>
              <div class="col-6">
                <Card />
              </div>
              <div class="col-6">
                <Card />
              </div>
            </div>
          </div>

          <div class="cover-carousel"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Decoration from "../ComponentsDecoration/Decoration.vue";
import Card from "../Main/Card.vue";
export default {
  name: "MainYourWeb",
  components: {
    Decoration,
    Card,
  },
  data() {
    return {
      groupList: [
        {
          id: "01",
          url: "Group-36-2x.png",
        },
        {
          id: "02",
          url: "Group-35-2x.png",
        },
        {
          id: "03",
          url: "Group-40-2x.png",
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
</style>

