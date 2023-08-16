<template>
  <img :src="image" alt="" />
</template>

<script>
export default {
  name: "AboutImg.vue",
  props: {
    image: String,
  },
};
</script>

<style lang="sass" scoped>
img
  position: absolute
  width: 488px
</style>
