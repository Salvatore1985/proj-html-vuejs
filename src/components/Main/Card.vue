<template>
  <div class="d-flex flex-wrap align-content-center">
    <section class="p-3 shadow" v-for="(card, index) in listCard" :key="index">
      <p class="p-3">{{ card.icons }}</p>
      <h4 class="p-3">{{ card.text }}</h4>
      <p class="p-3">
        {{ card.description }}
      </p>
    </section>
  </div>
</template>

<script>
export default {
  name: "MainCard",
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