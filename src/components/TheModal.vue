/* eslint-disable */
<template>
  <div v-if="show" class="modal-shadow" @click.self="closeModal">
    <div class="modal">
      <slot name="body">
        <form action="./TheHeader.vue" class="modal-form" :class="active">
          <p class="form-title">
            Заполните <span>форму</span> и мы обязательно свяжемся с Вами.
          </p>
          <input type="text" placeholder="Ваше имя..." required />
          <input type="text" placeholder="Ваш телефон..." required />
          <input type="textarea" placeholder="Комментарий..." required />
          <a class="button" type="submit" @click="showModal">
            Оставить заявку
          </a>
        </form>
      </slot>
      <TheModalThanks ref="modal"></TheModalThanks>
    </div>
  </div>
</template>

<script>
import TheModalThanks from "./TheModalThanks.vue";
export default {
  name: "ModalWindow",
  components: {
    TheModalThanks,
  },
  data: function () {
    return {
      show: false,
      active: true,
    };
  },
  methods: {
    closeModal: function () {
      this.show = false;
    },
    showModal: function () {
      this.$refs.modal.show = true;
    },
  },
};
</script>

<style lang="sass">
.hello
  color: #000
.modal-shadow
  position: absolute
  top: 0
  left: 0
  min-height: 100vw
  width: 100%
  background: rgba(0, 0, 0, 0.39)
  .modal
    width: 400px
    height: 530px
    font-size: 24px
    font-weight: 500
    text-align: center
    border-radius: 30px
    background: #f6faff
    padding: 20px 32px
    margin: 0 auto
    margin-top: 100px
    .modal-form
      .form-title
        padding-bottom: 32px
        margin: 0 auto
        width: 55%
  input
    width: 335px
    height: 60px
    border: none
    outline: none
    border-radius: 15px
    background: #FFF
    box-shadow: 0px 20px 45px -15px rgba(0, 0, 0, 0.05)
    background: #fff
    margin-bottom: 12px
    padding-left: 20px
    &[type=textarea]:nth-child(4)
      margin-bottom: 52px
      width: 336px
      height: 120px
    &::placeholder
      color: #C2C2C2
      font-size: 18px
      font-weight: 300
  span
    color: #018FA3
</style>
