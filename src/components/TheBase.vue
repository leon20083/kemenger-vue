<template>
  <!-- Начало: Данный блок удалять нельзя -->
  <div class="maketforfigma">
    <a href="https://t.me/s/FigmaToHTML" target="_blank">
      <img src="../assets/logo.png" />
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
</template>

<script>
export default {
  name: "TheBase",
};
</script>

<style lang="sass" scoped>
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
  padding: 10px 10px
  line-height: 0.70rem

.maketforfigma p > a
  color: #bbe4f0
  font-weight: bold

.maketforfigma p > a:hover
  color: #ffffff

.main
  flex: 1 0 auto

html
  height: 100%
</style>
