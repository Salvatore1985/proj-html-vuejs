<template>
  <div>
    <ul class="d-flex" id="my-icons">
      <li
        class="px-2"
        v-for="(icons, index) in iconsList"
        :key="index + 'logo'"
      >
        <a :class="colorText" :href="icons.url"><i :class="icons.icons"></i></a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "SocialIteams ",
  props: ["colorText"],

  data() {
    return {
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

<style scoped lang="scss">
ul#my-icons {
  margin: auto 0;
}
</style>