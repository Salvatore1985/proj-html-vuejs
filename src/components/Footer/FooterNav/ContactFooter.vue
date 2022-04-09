<template>
  <section class="p-2">
    <h3>{{ wrappedcontact[0] }}</h3>
    <Decoration class="py-3" />
    <ul class="ps-0" v-for="(element, index) in wrappedcontact" :key="index">
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
section {
  height: 380px;
}
</style>