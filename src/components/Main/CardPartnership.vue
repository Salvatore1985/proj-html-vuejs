<template>
  <div class="d-flex flex-wrap justify-content-evenly">
    <section
      :class="
        card.bgColor === 'black'
          ? 'my-bg-black-gray'
          : card.bgColor === 'green'
          ? 'my-bg-green'
          : ''
      "
      class="p-3 shadow text-center text-white"
      v-for="(card, index) in listCard"
      :key="index"
    >
      <p class="p-3">{{ card.request }}</p>
      <h4 class="p-3">{{ card.text }}</h4>
      <Button :className="'green'" :textbtn="'start now'" />
      <!--  <button class="rounded-pill border-0 gray px-4 shadow" type="submit">
        read more
      </button> -->
    </section>
  </div>
</template>

<script>
/* import ButtonSubmit from "@/Main/ButtonSubmit.vue"; */
import Button from "../Button/Button.vue";
export default {
  name: "CardPartnership",
  components: {
    Button,
  },
  props: ["listCard"],
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
section {
  width: calc(50% - 2.3rem);
  height: 350px;

  background-color: white;
  border-radius: 1rem;
}
</style>