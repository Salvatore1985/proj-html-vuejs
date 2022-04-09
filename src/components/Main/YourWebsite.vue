<template>
  <section class="">
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-5 d-flex flex-column justify-content-center">
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
            <Button :className="'green'" :textbtn="'read more'" />
          </div>
        </div>
        <div class="col-7">
          <div class="container-fluid">
            <div class="row my-card">
              <div class="col-12 d-flex justify-content-center">
                <!-- card -->
                <Card :listCard="cardsList" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Decoration from "../ComponentsDecoration/Decoration.vue";
import Card from "../Main/Card.vue";
import Button from "../Button/Button.vue";
export default {
  name: "MainYourWeb",
  components: {
    Decoration,
    Card,
    Button,
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
      cardsList: [
        {
          icons: "fas fa-tachometer-alt",
          text: "speed optimazation",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
        {
          icons: "fas fa-cloud",
          text: "cloud solutions",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
        {
          icons: "fas fa-tablet-alt",
          text: "website design",
          description:
            " Lorem ipsum dolor sit amet consectetur, adipisicing elit. Distinctio porro officiis itaque nesciunt, minima laudantium,",
        },
        {
          icons: "far fa-clock",
          text: "online marketing",
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

