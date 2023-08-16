<!-- eslint-disable prettier/prettier -->
<template>
  <div class="catalog-item">
    <div class="item-text">
      <div class="item-header" :style="{ background: color }">
        <p>{{ itemHeadTitle }}</p>
      </div>
      <h4>{{ itemTitle }}</h4>
      <ul v-if="!show" class="very-height">
        <li v-for="item of itemsText[numArr]" :key="item.id" class="fade-enter">
          {{ item }}
        </li>
      </ul>
      <ul v-else>
        <li
          v-for="item of itemsText[numArr].slice(0, 5)"
          :key="item.id"
          class="fade-enter"
        >
          {{ item }}
        </li>
      </ul>
      <a type="submit" @click="show = !show">Подробнее...</a>
    </div>
    <a href="./" class="button" :style="{ background: color }">Выбрать</a>
  </div>
</template>

<script>
export default {
  name: "CatalogItem",
  data() {
    return {
      show: true,
      itemsText: [
        [
          "4-6 лет",
          "3 занятия в неделю по 3 ч.",
          "Обучение чтению",
          "Письмо",
          "Математика",
          "Английский язык",
          "Развитие речи",
          "Концентрация внимания",
          "Усвоение изучаемого материала",
          "Различные техники запоминания",
          "Развитие логико-математического мышления",
        ],
        [
          "6-15 лет",
          "3 занятия в неделю по 1 ч.",
          "Увеличение скорости чтения",
          "Артикуляция",
          "Развитие речи",
          "Развитие внимания",
          "Увеличение поля зрения",
          "Увеличение словарного запаса",
          "Понимание прочитанного",
          "Пересказ",
          "Различные техники понимания",
          "Пробный урок и диагностика БЕСПЛАТНО",
        ],
        [
          "",
          "2 занятия в неделю по 1 ч.",
          "Быстрый счет",
          "Развитие высокой концентрации",
          "Увеличесние поля зрения",
          "Фотографическая память",
          "Пробный урок БЕСПЛАТНО",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
          "",
        ],
        [
          "3 занятия в неделю по 1 ч.",
          "Развитие памяти",
          "Восприятие пространства",
          "Прокачивание мелкой моторики",
          "Основы грамотного письма",
          "Развитие физической выносливости и усидчивости",
          "Умение писать диктанты без графических и орфографических ошибок",
        ],
        [
          "",
          "2 занятия в неделю по 1,5 ч.",
          "Чтение по правилам",
          "Знание 500 новых слов",
          "Самостоятельное выполнение домашнего задания",
          "",
          "",
          "",
          "",
          "",
          "",
        ],
        [
          "5 раз в неделю",
          "1 смена с 9:00 по 12:00",
          "2 смена с 14:00 по 17:00",
          "Проработка пробелов в знаниях",
          "Индивидуальный подход",
          "Выявление сильных сторон ребенка",
          "Профессиональная помощь в подготовке домашних заданий",
          "Дополнительные образовательные дисциплины",
          "",
          "",
          "",
        ],
      ],
    };
  },
  methods: {
    idArrNumber() {
      this.counter = this.counter + 1;
    },
    togleClass() {
      document.querySelectorAll(".item-text").addClass("very-heigth");
    },
  },
  props: {
    itemTitle: String,
    itemHeadTitle: String,
    color: String,
    numArr: String,
    text: String,
  },
};
</script>

<style lang="sass" scoped>
.fade-enter
  transition: opacity .5s

.fade-enter
  opacity: 1
.very-height
  height: 650px
.catalog-item
  position: relative
  text-align: center
  width: 387px
  padding-bottom: 60px
  background: #fff
  border-radius: 30px 30px 0px 0px
  margin: 0 auto
  min-height: 717px
  li
    font-size: 24px
    padding-bottom: 24px
    list-style: none
  h4
    font-size: 48px
    font-weight: 600
    padding-bottom: 24px

  a
    position: absolute
    bottom: 230px
    color: #018FA3
    font-size: 24px
    cursor: pointer
    left: 0
    right: 0
  .item-text
    padding-bottom: 140px
    display: flex
    flex-direction: column
    margin-bottom: 60px
    .item-header
      height: 80px
      flex-shrink: 0
      border-radius: 30px 30px 0px 0px
      display: flex
      justify-content: center
      align-items: center
      font-size: 24px
      font-weight: 700
      color: #fff
      margin-bottom: 60px
      text-transform: uppercase
  .button
    padding: 20px 60px !important
    color: #fff
    position: absolute
    bottom: 60px
    left: 0
    right: 0
    margin: 0 auto
    width: 30%
</style>
