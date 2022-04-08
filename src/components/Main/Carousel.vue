<template>
  <section class="bg_primary">
    <div class="container-fluid">
      <div class="row align-items-center position-relative">
        <div class="col-5 ps-5 py-5">
          <div>
            <h5 class="text-text-uppercase">17 years of experience</h5>
            <h1>We Are a</h1>
            <h1>
              Web Design <span class="text_color_color_primary">Agency</span>
            </h1>
          </div>
          <!-- Aggiunto componente style  -->
          <Decoration class="py-3" />
          <div>
            <p class="py-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae
              voluptatem explicabo voluptate nobis? Cum praesentium optio
              deleniti blanditiis veniam. Neque, dolorem! Asperiores accusamus
              vero quidem eaque natus reprehenderit cupiditate beatae.
            </p>
            <button class="rounded-pill border-0 gray" type="submit">
              read more
            </button>
          </div>

          <div class="py-5 d-flex justify-content-between align-items-center">
            <h6 class="text-text-uppercase">
              facebook - instagram - youtube - twitter
            </h6>
            <!-- bottone carosello -->
            <div class="d-flex wapped-carousel rounded-pill">
              <div
                class="btn-carousel rounded-pill"
                v-for="(element, index) in groupList"
                :key="index + 'group'"
              >
                <span @click="changeImg(index)">{{ element.id }}</span>
              </div>
            </div>
          </div>
        </div>
        <div class="col-8 offset-4 d-flex position-absolute top-0 p-0">
          <div class="cover-carousel">
            <img src="@/assets/images/Group-36-2x.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Decoration from "@/components/ComponentsDecoration/Decoration.vue";
export default {
  name: "MainCarousel",
  components: {
    Decoration,
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
  height: $carousel_height;
  z-index: 1;
  div {
    h1 {
      font-size: 4.5rem;
    }
    h5 {
      color: #00d9a6;
    }
  }
}
.wapped-carousel {
  background-image: linear-gradient(to right, #494949, #2e2e2e);
  padding: 0.25rem;
  position: relative;
  left: 18%;
  div {
    span {
      cursor: pointer;
    }
  }
  .btn-carousel {
    color: #aaaaaa;
    padding: 0.3rem 0.8rem;
  }
}
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

.btn-carousel:hover {
  background-image: linear-gradient(to right, #00d9a6, #b0f89b);
}
</style>

