<template>
  <section class="cover-carousel bg_primary">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-8">
          <div>
            <h5 class="text-text-uppercase">17 years of experience</h5>
            <h1>We Are a</h1>
            <h1>
              Web Design <span class="text_color_color_primary">Agency</span>
            </h1>
          </div>
          <!-- Aggiunto componente style  -->
          <Decoration />
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

          <div class="py-5 d-flex justify-content-between">
            <h6 class="text-text-uppercase">
              facebook - instagram - youtube - twitter
            </h6>
            <!-- bottone carosello -->
            <div class="d-flex wapped-carousel rounded-pill">
              <div class="btn-carousel rounded-pill">
                <span>01</span>
              </div>
              <div class="btn-carousel rounded-pill">
                <span class="">02</span>
              </div>
              <div class="btn-carousel rounded-pill">
                <span>03</span>
              </div>
            </div>
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
      /* socialCarousel: ["facebook", "instagram", "youtube", "twitter"], */
    };
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
.row {
  border: 1px solid red;
  height: 700px;
}
section {
  height: 700px;
}
.col-8 {
  border: 1px solid red;

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
  .btn-carousel {
    color: #aaaaaa;
    padding: 0.3rem 0.8rem;
  }
}
.cover-carousel {
  background-image: url("@/assets/images/Group-36-2x.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: 60%;
  background-position: 130% 50%;
}
.btn-carousel:hover {
  background-image: linear-gradient(to right, #00d9a6, #b0f89b);
}
</style>

