<template>
  <div class="item">
    <div class="user">
      <img :src="image" alt="" />
      <h5>{{ name }}</h5>
    </div>
    <p>{{ itemText }}</p>
  </div>
</template>

<script>
export default {
  name: "ReviewsItem",
  props: {
    itemText: String,
    image: String,
    name: String,
  },
};
</script>

<style lang="sass" scoped>
.item
  border-radius: 30px
  border: 4px solid #018FA3
  padding: 35px
  height: 215px
  width: 302px
  margin: 0 auto
  .user
    display: flex
    align-items: center
    padding-bottom: 12px
    h5
      font-size: 24px
    img
      width: 80px
      margin-right: 20px
  p
    font-size: 20px
    text-align: left
</style>
