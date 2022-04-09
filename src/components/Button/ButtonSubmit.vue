<template>
  <div>
    <div>
      <button :class="`rounded-pill border-0 ${className}`" type="submit">
        {{ textbtn }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ButtonSubmit",
  props: ["textbtn", "className"],

  data() {
    return {};
  },
};
</script>

<style>
</style>