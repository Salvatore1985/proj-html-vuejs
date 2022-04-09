<template>
  <div>
    <div class="container-fluid" id="footer-nav">
      <div class="row align-items-center">
        <div class="col-3 p-5">
          <LogoFooterCorporate :wrappedLogo="wrappedLogo" />
        </div>
        <div class="col-3 p-5">
          <LinkFooter :wrappedLink="wrappedLink" />
        </div>
        <div class="col-3 p-5">
          <ContactFooter :wrappedcontact="wrappedcontact" />
        </div>
        <div class="col-3 p-5">
          <LocationFooter :wrappedLocation="wrappedLocation" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LogoFooterCorporate from "../Footer/FooterNav/LogoFooterCorporate.vue";
import LinkFooter from "../Footer/FooterNav/LinkFooter.vue";
import ContactFooter from "../Footer/FooterNav/ContactFooter.vue";
import LocationFooter from "../Footer/FooterNav/LocationFooter.vue";
export default {
  name: "FooterNav",
  components: {
    LogoFooterCorporate,
    LinkFooter,
    ContactFooter,
    LocationFooter,
  },
  data() {
    return {
      wrappedLogo: [
        {
          logo: "cropped-Group-39-2x",
          url: "#",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia maximedistinctio corporis odit blanditiis soluta ipsum optio, providentillum omnis deserunt eaque ut eum autem velit vitae culpa consequatur?Harum!",
        },
      ],
      wrappedLink: [
        "quick links",

        {
          description: "careers",
          url: "#",
        },
        {
          description: "news",
          url: "#",
        },
        {
          description: "terms of use",
          url: "#",
        },
        {
          description: "privacy projects",
          url: "#",
        },
        {
          description: "about",
          url: "#",
        },
        {
          description: "contact",
          url: "#",
        },
      ],
      wrappedcontact: [
        "contact",
        "patricia c.amedee 4401 waldeck street grapevine nashville, TX 76051",
        "info@yourdomain.com",
        "+99 (0) 101 0000 888",
      ],
      wrappedLocation: [
        "location on map",
        {
          img: "map",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#footer-nav,
.row {
  height: 500px;
}
</style>