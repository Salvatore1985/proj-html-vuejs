<template>
  <section class="p-2">
    <h3>{{ wrappedLocation[0] }}</h3>
    <Decoration class="py-3" />
    <div class="ps-0 w-100">
      <img
        :src="require(`@/assets/images/${wrappedLocation[1].img}.png`)"
        alt=""
      />
    </div>
  </section>
</template>

<script>
import Decoration from "../../ComponentsDecoration/Decoration.vue";
export default {
  name: "LocationFooter",
  props: ["wrappedLocation"],
  components: {
    Decoration,
  },
};
</script>


<style lang="scss" scoped>
section {
  height: 380px;

  img {
    width: 100%;
  }
}
</style>