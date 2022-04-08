<template>
  <section>
    <div class="container-fluid">
      <div class="row align-items-center">
        <div class="col-10 position-relative">
          <section class="position-relative my-bg-opacity-green behind">
            <img
              src="@/assets/images/busy-architect-PYVKWM4-1024x872.jpg"
              alt=""
            />
          </section>
          <section class="my-front shadow pb-5">
            <img
              class="shadow"
              src="@/assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg"
              alt=""
            />
          </section>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainImgOurMissions",
  components: {},
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
@import "@/components/style/main-style.scss";
section.behind {
  height: 50%;
  img {
    width: 100%;

    border-radius: 2rem;
    position: relative;
    right: 12%;
  }
}
section.my-front {
  height: 50%;
  img {
    width: 100%;
    border-radius: 2rem;
    position: absolute;
    top: 15%;
    z-index: 1;
  }
}

.my-bg-opacity-green::before {
  content: "";
  display: block;
  width: 100%;
  height: 100%;
  background-image: linear-gradient(
    to top,
    rgba(177, 248, 155, 0.8),
    rgba(0, 217, 166, 0.8)
  );
  border-radius: 2rem;
  position: absolute;
  top: 0;
  right: 12%;
  z-index: 1;
}
</style>

