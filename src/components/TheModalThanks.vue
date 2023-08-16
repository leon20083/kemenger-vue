<template>
  <div v-if="show" class="modal-shadow" @click.self="closeModal">
    <div class="modal" @click="!showModal">
      <slot name="body">
        <div class="thanks">
          <img src="../assets/icon-thanks.png" alt="" />
          <p class="thanks-text"><span>Спасибо</span> за заявку</p>
          <p class="thanks-descr">
            В ближайшее время мы <span>свяжемся</span> с Вами
          </p>
        </div>
      </slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheModalThenks",
  data: function () {
    return {
      show: false,
    };
  },
  methods: {
    closeModal: function () {
      this.show = false;
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
.thanks
  font-size: 36px
  font-weight: 500
  padding: 80px 0 100px 0
  img
    width: 120px
    height: 120px
    margin-bottom: 16px
  .thanks-text, .thanks-descr
    margin: 0 auto
    width: 55% !important
    p
      width: 55% !important
  span
    color: #018FA3
</style>
