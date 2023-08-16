<template>
  <div class="about-top">
    <div class="container">
      <TheAboutTopLeft />
      <TheAboutTopRight />
    </div>
  </div>
</template>

<script>
import TheAboutTopLeft from "./TheAboutTopLeft.vue";
import TheAboutTopRight from "./TheAboutTopRight.vue";
export default {
  name: "AboutTop",
  components: {
    TheAboutTopLeft,
    TheAboutTopRight,
  },
};
</script>

<style lang="sass" scoped>
.about-top
  display: flex
  justify-content: space-between
</style>
