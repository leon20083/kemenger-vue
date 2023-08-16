<template>
  <!-- Начало: Данный блок удалять нельзя -->
  <div class="maketforfigma">
    <a href="https://t.me/s/FigmaToHTML" target="_blank">
      <img src="./assets/logo.png" />
    </a>
    <div>
      <p>
        Данная верстка, была реализована пользователем в рамках обучающего
        телеграм канал
        <a href="https://t.me/s/FigmaToHTML" target="_blank"
          >FIGMA | Макеты для верстки</a
        >
      </p>
      <p>
        При помощи
        <a href="https://t.me/HtmlCodeForMoney_bot?from_git" target="_blank"
          >Telegram-бота</a
        >
        пользователь получил оплату за верстку этого макета.
      </p>
    </div>
  </div>
  <!-- Конец -->
  <TheMain />
</template>

<script>
import TheMain from "./components/TheMain.vue";

export default {
  name: "App",
  components: {
    TheMain,
  },
};
</script>

<style lang="sass">
.maketforfigma
  flex: 0 0 auto
  background: #313a46
  font-weight: bold
  display: flex

.maketforfigma img
  border-radius: 10px
  margin: 4px 0 0 4px

.maketforfigma p
  color: #98a6ad
  text-decoration: none
  letter-spacing: .01875rem
  font-size: .775rem
  padding: 10px
  line-height: 0.70rem

.maketforfigma p > a
  color: #bbe4f0
  font-weight: bold

.maketforfigma p > a:hover
  color: #ffffff

.main
  flex: 1 0 auto

html
  // height: 100%
  scroll-behavior: smooth
body
  height: 100%
  padding: 0
  margin: 0
  max-width: 1440px
  font-family: 'Commissioner', sans-serif
  font-weight: 400
  font-size: 14px
  color: #000

.container
  width: 1250px
  margin: 0 auto
  display: flex
  justify-content: space-between
  align-items: center
h1, h2, h3, h4
  font-weight: 600
a
  text-decoration: none
  font-weight: 500
  color: #000
  cursor: pointer
img
  width: 100%
*
  margin: 0
  padding: 0
.swiper-button-next, .swiper-button-prev
  color: #000
.swiper-button-next
  right: 10
.swiper-button-prev
  left: 10
</style>
