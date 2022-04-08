<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container-fluid px-5">
      <a class="navbar-brand" href="#">
        <img src="@/assets/images/cropped-Group-39-2x.png" alt="" />
      </a>

      <div class="collapse navbar-collapse flex-grow-0 text-uppercase">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li
            v-for="(link, index) in navLink"
            :key="index + 'link'"
            class="nav-item"
          >
            <a class="nav-link" aria-current="page" :href="link.url">{{
              link.name
            }}</a>
          </li>
        </ul>
      </div>

      <div class="d-flex">
        <button class="rounded-pill border-0 green" type="submit">
          purchase
        </button>
        <span class="nav-link"><a href="#">search</a> </span>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "HomeHeaderNav",

  data() {
    return {
      navLink: [
        {
          name: "home",
          url: "#",
        },
        {
          name: "about",
          url: "#",
        },

        {
          name: "services",
          url: "#",
        },
        {
          name: "showcase",
          url: "#",
        },
        {
          name: "blog",
          url: "#",
        },
        {
          name: "contact",
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
.navbar {
  background-color: $brand_secondary;
  height: $header_nav;
}
</style>
