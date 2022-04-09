<template>
  <div>
    <div>
      <button
        :class="`text-uppercase px-5 py-3 rounded-pill border-0 ${className} ${shadow}`"
        type="submit"
      >
        {{ textbtn }}
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ButtonSubmit",
  props: ["textbtn", "className", "shadow"],

  data() {
    return {};
  },
};
</script>
<style scoped lang="scss">
</style>
