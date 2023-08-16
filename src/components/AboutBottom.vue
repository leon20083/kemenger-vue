<template>
  <div class="about-bottom">
    <div class="container">
      <AboutBottomRight />
      <AboutBottomLeft />
    </div>
  </div>
</template>

<script>
import AboutBottomRight from "./AboutBottomRight.vue";
import AboutBottomLeft from "./AboutBottomLeft.vue";
export default {
  name: "AboutBottom",
  components: {
    AboutBottomRight,
    // eslint-disable-next-line vue/no-unused-components
    AboutBottomLeft,
  },
};
</script>

<style lang="sass" scoped>
.about-bottom
  display: flex
  justify-content: space-between
</style>
