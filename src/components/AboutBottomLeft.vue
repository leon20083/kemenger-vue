<template>
  <div class="about-bottom-left">
    <img src="../assets/circle2.svg" alt="" />
    <div class="about-bottom_text">
      <p>
        Наши ученики показывают результат уже с первого месяца работы, мы
        поддерживаем в нашем центре теплую и дружескую атмосферу Побывав у нас
        детям обязательно захочется вернуться сюда снова Развивайтесь вместе с
        нами
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutbottomLeft",
};
</script>

<style lang="sass" scoped>
.about-bottom-left
  margin-left: 60px
  position: relative
  .about-bottom_text
    position: relative
    width: 440px
    height: 175px
    flex-shrink: 0
    border-radius: 30px
    background: #FFF7BE
    left: -120px
    p
      position: absolute
      font-size: 24px
      left: -35px
      top: 35px
      padding-right: 15px
  img
    position: absolute
    width: 201px
    height: 200px
    bottom: -60px
    right: 60px
</style>
