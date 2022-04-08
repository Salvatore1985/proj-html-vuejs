<template>
  <section class="">
    <div class="container-fluid">
      <div class="row align-items-center p-5">
        <div class="col-6 d-flex flex-column justify-content-end">
          <Decoration class="py-3" />
          <div>
            <h1 class="py-3">
              our recent
              <span class="text_color_color_primary">web designs</span>
              & some examples of past
              <span class="text_color_color_primary">projects</span>
            </h1>
          </div>
          <!-- Aggiunto componente style  -->
          <Decoration class="py-3" />
        </div>
        <div class="col-6 d-flex align-items-end">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga hic
            recusandae eligendi officia impedit error provident, iste
            repudiandae eaque maxime quia possimus, incidunt illo in temporibus
            modi! Dolores, maiores nemo!
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Decoration from "../ComponentsDecoration/Decoration.vue";

export default {
  name: "ProjectsMain",
  components: {
    Decoration,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@import "@/components/style/main-style.scss";
.col-6 {
  height: $projects_main;

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

