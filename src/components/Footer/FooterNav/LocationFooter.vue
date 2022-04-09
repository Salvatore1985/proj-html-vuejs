<template>
  <section>
    <h3>{{ wrappedLocation[0] }}</h3>
    <Decoration class="py-3" />
    <div class="ps-0 pt-2">
      <img
        class="img-fluid"
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

<style>
</style>