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
            <ul class="d-flex" id="my-icons">
              <li
                class="px-2"
                v-for="(icons, index) in iconsList"
                :key="index + 'logo'"
              >
                <a :href="icons.url"><i :class="icons.icons"></i></a>
              </li>
            </ul>
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
          icons: "fab fa-facebook-f",
          url: "#",
        },
        {
          alt: "logo-twitter",
          icons: "fab fa-twitter",
          url: "#",
        },

        {
          alt: "pinterest",
          icons: "fab fa-pinterest-p",
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

ul#my-icons {
  margin: auto 0;
  a {
    color: white;
  }
}
</style>
