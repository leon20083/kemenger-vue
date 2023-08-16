<template>
  <div id="about" class="about">
    <div class="container">
      <div class="about-top">
        <AboutTop />
        <AboutBottom />
      </div>
    </div>
  </div>
</template>

<script>
import AboutTop from "./AboutTop.vue";
import AboutBottom from "./AboutBottom.vue";
export default {
  name: "TheAbout",
  components: {
    AboutTop,
    AboutBottom,
  },
};
</script>

<style lang="sass" scoped>
.about
  margin-bottom: 100px
  .about-top
    width: 100%
    position: relative
    display: flex
    flex-direction: column
</style>
