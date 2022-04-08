<template>
  <section>
    <div class="container-fluid py-3">
      <div class="row">
        <div
          class="
            col-12
            justify-content-center
            d-flex
            flex-wrap
            position-relative
          "
        >
          <div
            class="card border-0"
            v-for="(img, index) in imagArtistList"
            :key="index"
          >
            <img
              :src="require(`@/assets/images/${img.src}`)"
              :alt="img.imgName"
            />
          </div>
          <div id="wrapped-option">
            <!-- lista option -->
            <ul>
              <li
                class="py-1"
                v-for="(element, index) in optionImg"
                :key="index + 'buy'"
              >
                <a :href="element.url">
                  <div class="d-flex align-items-center px-2">
                    <span class="p-2">{{ element.icons }}</span>
                    <span class="">{{ element.text }}</span>
                  </div>
                </a>
              </li>
            </ul>
          </div>
          <div class="my-btn">
            <button class="rounded-pill border-0 green px-4" type="submit">
              read more
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ArtisticImages",
  data() {
    return {
      imagArtistList: [
        {
          src: "ina-soulis-227104-unsplash-1024x1024.jpg",
          imgName: "sunisa",
          id: "1",
        },
        {
          src: "sunisa-misa-531163-unsplash-1024x1024.jpg",
          imgName: "sunisa",
          id: "2",
        },
        {
          src: "355H-1024x1024.jpg",
          imgName: "sunisa",
          id: "3",
        },
        {
          src: "photo-1448932252197-d19750584e56-1024x1024.jpg",
          imgName: "sunisa",
          id: "4",
        },
        {
          src: "business-competition-PB366D8-1024x1024.jpg",
          imgName: "sunisa",
          id: "5",
        },
        {
          src: "cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg",
          imgName: "sunisa",
          id: "6",
        },
        {
          src: "aa9a4539-PQGJ7HU-1024x1024.jpg",
          imgName: "sunisa",
          id: "7",
        },
        {
          src: "cody-davis-253928-unsplash-1024x1024.jpg",
          imgName: "sunisa",
          id: "8",
        },
      ],
      optionImg: [
        {
          icons: "icons",
          text: "browse demos",
          url: "#",
        },
        {
          icons: "icons",
          text: "buy now!",
          url: "#",
        },
        {
          icons: "icons",
          text: "export section",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
img {
  width: 22.8rem;
  height: 100%;
  margin: 0.25rem;
  border-radius: 0.5rem;
}
ul {
  li {
    div {
      background-color: rgba(134, 134, 134, 0.8);
      border-radius: 1rem 0 0 1rem;
      span {
        color: #dbdbdb;
      }
    }
  }
}
#wrapped-option {
  position: absolute;
  top: 11.4rem;
  right: 0;
}
.my-btn {
  padding: 8rem 0 12rem 0;
}
</style>