<template>
  <div>
    <button class="rounded-pill border-0" type="submit">
      {{ textBtn(text) }}
    </button>
  </div>
</template>

<script>
export default {
  name: "ButtonSingle",

  data() {
    return {};
  },
  methods: {
    textBtn(text) {
      this.$emit("textBtn", text);
    },
  },
};
</script>

<style>
</style>