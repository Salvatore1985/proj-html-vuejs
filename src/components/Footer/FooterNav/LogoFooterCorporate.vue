<template>
  <div>
    <section v-for="(element, index) in wrappedLogo" :key="index">
      <div>
        <img :src="require(`@/assets/images/${element.logo}.png`)" alt="" />
        <!--  <img src="@/assets/images/cropped-Group-39-2x.png" alt="" /> -->
      </div>
      <div>
        <p class="py-4">
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

<style>
</style>