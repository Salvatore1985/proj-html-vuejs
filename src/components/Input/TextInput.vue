<template>
  <div>
    <div class="mb-3 d-flex justify-content-center">
      <input
        type="text"
        class="p-4 border-0"
        :placeholder="placeholder"
        aria-label="Recipient's username"
        aria-describedby="basic-addon2"
      />
      <span class="input-group-text border-0 text-uppercase px-4">{{
        submit
      }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "TextInput",
  props: ["submit", "placeholder"],
};
</script>

<style lang="scss" scoped>
div {
  width: 100%;
  input {
    border-radius: 50rem 0 0 50rem;
  }
  span {
    border-radius: 0 50rem 50rem 0;
  }
}
input,
span {
  background-color: #3c3c3c;
  color: #afafaf;
  cursor: pointer;
}
</style>