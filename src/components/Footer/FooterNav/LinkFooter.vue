<template>
  <section class="p-2">
    <h3>{{ wrappedLink[0] }}</h3>
    <Decoration class="py-3" />
    <ul class="py-4 ps-0">
      <li v-for="(element, index) in wrappedLink" :key="index">
        {{ element.description }}
      </li>
    </ul>
  </section>
</template>

<script>
import Decoration from "../../ComponentsDecoration/Decoration.vue";
export default {
  name: "LinkFooter",
  props: ["wrappedLink"],
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