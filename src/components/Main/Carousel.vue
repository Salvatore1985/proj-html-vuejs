<template>
  <section class="bg_primary">
    <div class="container-fluid">
      <div class="row align-items-center position-relative">
        <div class="col-5 ps-5 py-5">
          <div>
            <h5 class="text-text-uppercase">17 years of experience</h5>
            <h1 class="py-3">We Are a</h1>
            <h1>
              Web Design <span class="text_color_color_primary">Agency</span>
            </h1>
          </div>
          <!-- Aggiunto componente style  -->
          <Decoration class="py-3" />
          <div class="py-4">
            <p class="py-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae
              voluptatem explicabo voluptate nobis? Cum praesentium optio
              deleniti blanditiis veniam. Neque, dolorem! Asperiores accusamus
              vero quidem eaque natus reprehenderit cupiditate beatae.
            </p>
            <Button :className="'gray'" :textbtn="'read more'" />
          </div>

          <div class="py-5 d-flex justify-content-between align-items-center">
            <h6 class="text-text-uppercase">
              facebook - instagram - youtube - twitter
            </h6>
            <!-- bottone carosello -->
            <div class="d-flex wapped-carousel rounded-pill my-shadow-lg">
              <div
                @click="getSlide(index)"
                :class="visibleCover == index ? 'active' : ''"
                class="btn-carousel rounded-pill fs-4 px-3"
                v-for="(element, index) in groupList"
                :key="index + 'group'"
              >
                <span>{{ element.id }}</span>
              </div>
            </div>
          </div>
        </div>
        <div class="col-8 offset-4 d-flex position-absolute top-0 p-0">
          <div
            class="cover-carousel"
            :class="visibleCover == index ? 'active' : ''"
            v-for="(cover, index) in groupList"
            :index="visibleCover"
            :key="index"
          >
            <img
              :src="require(`../../assets/images/${cover.url}`)"
              :alt="cover.text"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Decoration from "../ComponentsDecoration/Decoration.vue";
import Button from "../Button/Button.vue";

export default {
  name: "MainCarousel",
  components: {
    Decoration,
    Button,
  },
  data() {
    return {
      visibleCover: 0,
      indexBtn: 0,
      groupList: [
        {
          id: "01",
          url: "Group-36-2x.png",
          text: "Group-36-2x",
        },
        {
          id: "02",
          url: "Group-35-2x.png",
          text: "Group-35-2x",
        },
        {
          id: "03",
          url: "Group-40-2x.png",
          text: "Group-40-2x",
        },
      ],
    };
  },
  methods: {
    getSlide(index) {
      this.visibleCover = index;
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
      font-size: 3.8rem;
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
  display: none;

  img {
    width: 1200px;
    height: $carousel_height;
    object-fit: cover;
    object-position: center;
    object-position: right;
    position: absolute;
  }
}
.cover-carousel.active {
  display: block;
}
.btn-carousel.active {
  background-image: linear-gradient(to right, #00d9a6, #b0f89b);
}
</style>

