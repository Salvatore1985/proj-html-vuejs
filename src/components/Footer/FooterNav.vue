<template>
  <div>
    <div class="container-fluid" id="footer-nav">
      <div class="row align-items-center justify-content-center">
        <div class="col-12">
          <LogoFooterCorporate :wrappedLogo="wrappedLogo" />
        </div>
        <div class="col-12">
          <LinkFooter :wrappedLink="wrappedLink" />
        </div>
        <div class="col-12">
          <ContactFooter :wrappedcontact="wrappedcontact" />
        </div>
        <div class="col-12">
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
            "While the lovly valley teems with vapour around me, and the meridian sun strikes the upper sorfuce of the impenetrable foliage of my trees. While the lovly valley teems with vopur around me. ",
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
  .col-12 {
    width: calc(100% / 4);
  }
}
</style>