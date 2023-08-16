<template>
  <div class="title">
    <h2>{{ title }}</h2>
  </div>
</template>

<script>
export default {
  name: "TheTitle",
  props: {
    title: String,
  },
};
</script>

<style lang="sass" scoped>
.title
  font-size: 48px
  margin-top: 70px
  margin-bottom: 70px
  text-align: center
</style>
