<template>
  <div class="main">
    <TheHeader />
    <TheAbout />
    <TheDirection />
    <TheCatalog />
    <TheOurCertificates />
    <TheReviews />
    <TheContact />
    <TheMaps />
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from "./TheHeader.vue";
import TheAbout from "./TheAbout.vue";
import TheDirection from "./TheDirection.vue";
import TheCatalog from "./TheCatalog.vue";
import TheOurCertificates from "./TheOurCertificates.vue";
import TheReviews from "./TheReviews.vue";
import TheContact from "./TheContact.vue";
import TheMaps from "./TheMaps.vue";
import TheFooter from "./TheFooter.vue";
export default {
  name: "TheMain",
  components: {
    TheHeader,
    TheAbout,
    TheDirection,
    TheCatalog,
    TheOurCertificates,
    TheReviews,
    TheContact,
    TheMaps,
    TheFooter,
  },
};
</script>

<style lang="sass"></style>
