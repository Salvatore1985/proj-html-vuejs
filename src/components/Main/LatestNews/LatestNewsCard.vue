<template>
  <section>
    <div class="container-fluid py-3">
      <div class="row">
        <div class="col-12 justify-content-evenly d-flex flex-wrap">
          <div
            class="position-relative"
            v-for="(img, index) in listCard"
            :key="index"
          >
            <div class="shadow">
              <img
                :src="require(`@/assets/images/${img.src}`)"
                :alt="img.new"
              />
            </div>
            <div id="wrapped-new" class="shadow">
              <ul>
                <li>
                  <div class="px-2">
                    <h6 class="pt-5">{{ img.date }}</h6>
                    <h4 class="position-relative">
                      <span class="decoration-style-point text-capitalize">{{
                        img.new
                      }}</span>
                    </h4>
                  </div>
                </li>
              </ul>
            </div>
          </div>
          <div id="wrapped-new"></div>
          <div class="my-btn">
            <Button
              :className="'gray'"
              :textbtn="'veiw all post'"
              :shadow="'shadow-lg'"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Button from "../../Button/Button.vue";
export default {
  name: "LatestNewsCard",
  props: ["listCard"],
  components: {
    Button,
  },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
div {
  border-radius: 0.5rem;

  img {
    width: 29.3rem;
    height: 100%;
    border-radius: 0.5rem;
  }
}
h6 {
  color: gray;
}
div#wrapped-new {
  background-color: white;
  border-radius: 0.5rem;
  position: absolute;
  width: 90%;
  bottom: -10%;
  left: 50%;
  transform: translate(-50%);
}

.my-btn {
  padding: 8rem 0 12rem 0;
}
</style>