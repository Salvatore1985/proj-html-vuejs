<template>
  <nav>
    <section class="header-social">
      <div class="container-fluid text-white">
        <div class="row justify-content-between px-5" id="row-social">
          <!-- Cod-Page -->
          <div class="col-6 d-flex align-items-center">
            <ul
              class="nav"
              v-for="(cod, index) in codPage"
              :key="index + 'cod'"
            >
              <li class="pe-1 nav-item">{{ cod.page }}</li>
              <li class="pe-3 nav-item">{{ cod.codPrimary }}</li>
              <li class="nav-item">{{ cod.codSecondary }}</li>
            </ul>
          </div>
          <!-- social -->
          <div class="col-6 d-flex align-items-center justify-content-end">
            <span>prova</span>
          </div>
        </div>
      </div>
    </section>
    <section class="header-nav"></section>
  </nav>
</template>

<script>
export default {
  name: "HomeHeaderSocial",
  data() {
    return {
      codPage: [
        {
          page: "(001)",
          codPrimary: "88451234",
          codSecondary: "88455438",
        },
      ],
      iconsList: [
        {
          alt: "facebook",
          icons: "logo-facebook",
          url: "#",
        },
        {
          alt: "twitter",
          icons: "logo-twitter",
          url: "#",
        },

        {
          alt: "pinterest",
          icons: "logo-pinterest",
          url: "#",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/main-style.scss";
.header-social {
  background-color: $color_primary;
  height: $header_social;
}

.col-6 {
  height: $header_social;
}
</style>
