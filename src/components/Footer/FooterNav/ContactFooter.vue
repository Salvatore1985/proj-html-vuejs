<template>
  <section>
    <h3>{{ wrappedcontact[0] }}</h3>
    <Decoration class="py-3" />
    <ul
      class="ps-0 pt-2"
      v-for="(element, index) in wrappedcontact"
      :key="index"
    >
      <li class="p-0">
        {{ element }}
      </li>
    </ul>
  </section>
</template>

<script>
import Decoration from "../../ComponentsDecoration/Decoration.vue";
export default {
  name: "ContactFooter",
  props: ["wrappedcontact"],
  components: {
    Decoration,
  },
};
</script>

<style lang="scss" scoped>
/* section {
  max-height: 380px;
  border: 1px solid red;
} */
</style>