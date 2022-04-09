<template>
  <section class="my-bg-black-gray">
    <div class="container-fluid">
      <div class="row align-items-center px-3">
        <div class="col-12 d-flex justify-content-between">
          <div>
            <span class="text-secondary"> Ⓒ 2020 phlox business theme.</span>
          </div>
          <div>
            <Social :colorText="'text-secondary'" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Social from "../Social.vue";
export default {
  name: "FooterSocial",
  components: { Social },
};
</script>

<style scoped lang="scss">
section {
  height: 15vh;
  .row {
    height: 15vh;
  }
}
</style>