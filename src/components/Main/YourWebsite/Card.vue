<template>
  <div class="d-flex flex-wrap align-content-center">
    <section class="p-4 shadow" v-for="(card, index) in listCard" :key="index">
      <span><i class="py-2" :class="card.icons"></i></span>
      <h4 class="py-3 text-capitalize">{{ card.text }}</h4>
      <p>
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
section:hover {
  color: white;
  background-image: linear-gradient(to bottom left, #b0f89b, #00d9a6);
}
i {
  font-size: 3.5rem;
}
</style>