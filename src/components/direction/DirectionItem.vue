<template>
  <div class="direction-item">
    <img :src="image" alt="" />
    <p>{{ text }}</p>
    <!-- <about-img :image="this.ImageUrl"></about-img> -->
    <!-- <direction-item-text text="Группа продленного дня"></direction-item-text> -->
  </div>
</template>

<script>
// import AboutImg from "../about/AboutImg";
// import DirectionItemText from "./DirectionItemText.vue";
export default {
  name: "DirectionItem",
  components: {
    // DirectionItemText,
    // AboutImg,
  },
  props: {
    image: String,
    text: String,
  },
  data() {
    return {
      ImageUrl: require("../../assets/icons/after-school-club.png"),
    };
  },
};
</script>

<style lang="sass" scoped>
.direction-item
  display: flex
  flex-direction: column
  justify-content: space-around
  align-items: center
  height: 200px
  width: 100px
  margin: 0 auto
  text-align: center
  margin-top: 30px
  img
    width: 120px
    height: 120px
    position: relative
  p
    font-size: 24px
    padding-bottom: 26px
</style>
