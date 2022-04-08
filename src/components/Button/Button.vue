<template>
  <div>
    <button class="rounded-pill border-0" type="submit">
      {{ textbtn }}
    </button>
  </div>
</template>

<script>
export default {
  name: "ButtonSingle",
  props: ["textbtn"],

  data() {
    return {};
  },
};
</script>

<style>
</style>