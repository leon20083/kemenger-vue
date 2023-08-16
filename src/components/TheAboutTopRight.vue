<template>
  <div class="about-top-right">
    <!-- <img src="../assets/kids-1.png" alt="" /> -->
    <about-img :image="this.src"></about-img>
    <about-div></about-div>
  </div>
</template>
<script>
import AboutImg from "./about/AboutImg";
import AboutDiv from "./about/AboutDiv.vue";
export default {
  name: "TheAboutTopRight",
  data() {
    return {
      src: require("../assets/kids-2.png"),
    };
  },
  components: {
    // eslint-disable-next-line vue/no-unused-components
    AboutImg,
    AboutDiv,
  },
};
</script>
<style lang="sass" scoped>
.about-top-right
  position: relative
  img
    right: 30px
  div
    top: 30px
</style>
