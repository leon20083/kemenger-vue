<template>
  <div class="contacts" id="contacts">
    <div class="container">
      <div class="contact-left">
        <div class="img-contact"></div>
        <TheTitle title="Наши контакты" />
        <h5>
          Запишитесь на бесплатный пробный урок<br />
          по номеру:
        </h5>
        <p>8 (771) 145-98-26</p>
        <h5>Адрес:</h5>
        <p>г. Нур-Султан, ул. К. Аманжолова, 28, офис 14</p>
        <h5>График работы:</h5>
        <ul>
          <li>Пн-Пт - 9:00-19:00;</li>
          <li>Сб - 9:00-17:00;</li>
          <li>Вс - выходной</li>
        </ul>
        <h5>E-mail:</h5>
        <p>@kemenger.mektebi</p>
      </div>
      <div class="contact-right">
        <img src="../assets/boys.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import TheTitle from "./TheTitle.vue";
export default {
  name: "TheContact",
  components: {
    TheTitle,
  },
};
</script>

<style lang="sass" scoped>
.contacts
  font-size: 24px
  z-index: 1
  padding-bottom: 80px
  .container
    // width: 1150px !important
  .title
    margin: 0
  .contact-left
    position: relative
    border-radius: 30px
    background: #018FA3
    box-shadow: 0px 50px 50px -27px rgba(0, 0, 0, 0.10)
    color: #FFF
    padding: 12px 42px 38px
    margin-top: 130px
    margin-left: 50px
    .img-contact
      position: absolute
      background: #95D8E0
      border-radius: 10em
      left: 35px
      top: -55px
      width: 200px
      height: 200px
      z-index: -2
    .h5
      padding-bottom: 8px
    p
      padding-bottom: 20px
    ul
      padding-bottom: 8px
      li
        list-style: none
</style>
