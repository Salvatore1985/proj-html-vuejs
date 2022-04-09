<template>
  <section class="bg_primary">
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-7">
          <ImgOurMissions />
        </div>
        <div class="col-5 p-5 d-flex flex-column justify-content-center">
          <div>
            <h1 class="py-3">
              learn more about our
              <span class="text_color_color_primary">missions</span>
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
            <Button :className="'green'" :textbtn="'read more'" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Decoration from "../ComponentsDecoration/Decoration.vue";
import ImgOurMissions from "./ImgOurMissions.vue";
import Button from "../Button/Button.vue";
export default {
  name: "MainOurMissions",
  components: {
    Decoration,
    ImgOurMissions,
    Button,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@import "@/components/style/main-style.scss";
.col-5 {
  height: $our_missions;

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

