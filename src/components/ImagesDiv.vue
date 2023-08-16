<template>
  <div class="img-wrapper">
    <img :src="image" alt="" />
  </div>
</template>

<script>
export default {
  name: "ImagesDiv",
  props: {
    image: String,
  },
};
</script>

<style lang="sass" scoped></style>
