<template>
  <div class="d-flex flex-wrap align-content-center">
    <section class="p-3 shadow" v-for="(card, index) in listCard" :key="index">
      <p class="p-3">{{ card.request }}</p>
      <h4 class="p-3">{{ card.text }}</h4>

      <button class="rounded-pill border-0 gray px-4 shadow" type="submit">
        read more
      </button>
    </section>
  </div>
</template>

<script>
export default {
  name: "CardPartnership",
  props: ["listCard"],
};
</script>

<style lang="scss" scoped>
section {
  width: calc(50% - 2.5rem);
  height: 300px;
  margin: 1rem;
  background-color: white;
  border-radius: 1rem;
}
</style>