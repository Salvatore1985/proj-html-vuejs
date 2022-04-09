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
      class="p-3 shadow text-center text-white my-card"
      v-for="(card, index) in listCard"
      :key="index"
    >
      <p class="p-3">{{ card.request }}</p>
      <h4 class="p-3">{{ card.text }}</h4>
      <section class="d-flex flex-column align-items-center">
        <Button
          class="py-3"
          v-if="card.input === 'button'"
          :className="'gray'"
          :textbtn="'start now'"
          :shadow="'shadow-lg'"
        />
        <TextInput
          class="py-3"
          v-if="card.input === 'text'"
          :placeholder="'Enter Your Email Address'"
          :submit="'submit'"
        />
      </section>
    </section>
  </div>
</template>

<script>
import Button from "../../Button/Button.vue";
import TextInput from "../../Input/TextInput.vue";
export default {
  name: "CardPartnership",
  components: {
    Button,
    TextInput,
  },
  props: ["listCard"],
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
section.my-card {
  width: calc(50% - 2.3rem);
  height: 350px;

  background-color: white;
  border-radius: 1rem;
}
</style>