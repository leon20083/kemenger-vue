<template>
  <div class="about-top-left">
    <img src="../assets/circle.svg" alt="" />
    <div class="about-top_text">
      <p>
        В нашем центре работают профессиональные педагоги любящие детей и
        преданные своему делу. Мы помогаем детям совершенствовать свои
        интеллекуальные способности чтобы они могли познавать мир и делать его
        более красивым и добрым.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheAboutTopLeft",
};
</script>

<style lang="sass" scoped>
.about-top-left
  margin-left: 60px
  .about-top_text
    position: relative
    width: 440px
    height: 204px
    flex-shrink: 0
    border-radius: 30px
    background: #FFF7BE
    left: 120px
    p
      position: absolute
      font-size: 24px
      left: -35px
      top: 35px
      padding-right: 10px
  img
    position: absolute
    width: 201px
    height: 200px
    top: 0
    left: 75px
</style>
