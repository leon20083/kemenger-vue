<template>
  <header class="header">
    <div class="head-top">
      <div class="container">
        <div class="logo"><img src="../assets/logo-main.png" alt="" /></div>
        <div class="top-menu">
          <ul>
            <li><a href="#about">О нас</a></li>
            <li><a href="#catalog">Каталог</a></li>
            <li><a href="#certificates">Сертификаты</a></li>
            <li><a href="#reviews">Отзывы</a></li>
            <li><a href="#contacts">Контакты</a></li>
          </ul>
        </div>
        <div class="phone">
          <img src="../assets/phone.png" alt="" />
          <strong>8 (771) 145-98-26</strong>
        </div>
      </div>
    </div>
    <div class="header-text">
      <div class="container">
        <h1>
          <span>KEMENGER MEKTEBI</span> - центр<br />
          интеллектуального развития
        </h1>
        <p>
          Обучение происходит на казахском и русском языках. При записи на два
          или более курсов предусмотрена скидка. Запишитесь на бесплатный
          пробный урок.
        </p>
        <a class="button show-modal-button" @click="showModal" type="submit"
          >Оставить заявку</a
        >
        <the-modal ref="modal"> </the-modal>
      </div>
    </div>
  </header>
</template>

<script>
import TheModal from "./TheModal.vue";
export default {
  name: "TheHeader",
  components: {
    TheModal,
  },
  methods: {
    showModal: function () {
      this.$refs.modal.show = true;
    },
  },
};
</script>

<style lang="sass">
.header
  background: url(../assets/background-head.png) no-repeat center center
  // max-width: 1440px
  height: 100%
  -webkit-background-size: cover
  -moz-background-size: cover
  -o-background-size: cover
  background-size: cover
  padding-bottom: 260px
  .head-top
    margin-bottom: 156px
    .logo
      width: 20%
      img
        width: 102px
      height: 88px
    .top-menu
      width: 60%
      padding-right: 200px
      ul
        display: flex
        justify-content: space-between
        li
          list-style: none
    .phone
      width: 20%
      display: flex
      justify-content: flex-start
      align-items: center
      img
        width: 40px
        height: 40px
        margin-right: 10px
  .header-text
    font-size: 48px
    // margin-bottom: 185px
    .container
      flex-direction: column
      align-items: flex-start
      h1
        display: inline
        font-size: 48px
        margin-bottom: 45px
        span
          color:#018FA3
      p
        font-size: 24px
        width: 45%
        margin-bottom: 45px
      a
        padding: 21px 45px
        background: #FAE01A
        box-shadow: 0px 20px 40px -27px rgba(0, 0, 0, 0.15)
        border-radius: 10em
        font-size: 20px
        font-style: normal
        font-weight: 500
        line-height: normal
// .header
//   margin-bottom: 135px
</style>
