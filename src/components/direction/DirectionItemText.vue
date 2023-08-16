<template>
  <p>{{ text }}</p>
</template>

<script>
export default {
  name: "DirectionItemText",
  props: {
    text: String,
  },
};
</script>

<style lang="sass" scoped>
p
  text-align: center
  font-size: 24px
</style>
