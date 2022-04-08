<template>
  <section class="position-relative">
    <div class="my-bg-guest"></div>
    <div class="text-center">
      <span>❝</span>
      <p class="py-5">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consectetur
        doloribus sunt quisquam omnis est dolorum earum odio quibusdam fugiat,
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Consectetur
        doloribus sunt quisquam omnis est dolorum earum odio quibusdam fugiat
      </p>
      <div class="py-4">
        <img
          src="@/assets/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg"
          alt=""
        />
      </div>
      <h3>lissa durdin</h3>
      <pre>client</pre>
    </div>
  </section>
</template>

<script>
export default {
  name: "JumbotronGuest",
};
</script>

<style lang="scss" scoped>
section {
  div.my-bg-guest {
    width: 100vw;
    height: 800px;
    background-image: url("@/assets/images/four-businesspeople-in-a-boardroom-with-paperwork-PC4V8H4.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    filter: opacity(80%);
  }

  div.text-center {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    width: 50%;
    margin: auto 0;
    span {
      font-size: 8rem;
      color: #00d9a6;
    }
    h3 {
      color: #00d9a6;
    }
  }
}
img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid white;
}
.my-bg-guest::after {
  content: "";
  display: block;
  width: 100%;
  height: 100%;
  background-color: rgba(17, 13, 7, 0.8);
  position: absolute;
  top: 0;
  left: 0;
}
</style>