<template>
  <div>
    <section class="p-2" v-for="(element, index) in wrappedLogo" :key="index">
      <div class="pb-4">
        <img :src="require(`@/assets/images/${element.logo}.png`)" alt="" />
        <!--  <img src="@/assets/images/cropped-Group-39-2x.png" alt="" /> -->
      </div>
      <div>
        <p>
          {{ element.description }}
        </p>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "LogoFooter",
  props: ["wrappedLogo"],
};
</script>

<style lang="scss" scoped>
section {
  height: 380px;
}
</style>