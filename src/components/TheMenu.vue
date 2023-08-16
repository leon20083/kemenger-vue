<template>
  <div class="top-menu">
    <ul>
      <li><a href="#about">О нас</a></li>
      <li><a href="#catalog">Каталог</a></li>
      <li><a href="#certificates">Сертификаты</a></li>
      <li><a href="#reviews">Отзывы</a></li>
      <li><a href="#contacts">Контакты</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "TheMenu",
};
</script>

<style lang="sass" scoped>
.top-menu
  width: 60%
  padding-right: 200px
  ul
    display: flex
    justify-content: space-between
    li
      list-style: none
      a
        color: #fff !important
</style>
