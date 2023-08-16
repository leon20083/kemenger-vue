<template>
  <div class="direction">
    <div class="container">
      <div class="direction-left">
        <DirectionItem
          :image="this.imageUrl.mentalArithmetic"
          :text="this.textItem.item1"
        />
        <DirectionItem
          :image="this.imageUrl.speedReading"
          :text="this.textItem.item2"
        />
        <DirectionItem
          :image="this.imageUrl.preparationForSchool"
          :text="this.textItem.item3"
        />
      </div>
      <div class="direction-center">
        <img src="../assets/direction.png" alt="" />
        <direction-item-text :text="this.text"></direction-item-text>
        <DirectionItem
          :image="this.imageUrl.afterSchoolClub"
          :text="this.textItem.item7"
        />
      </div>
      <div class="direction-right">
        <DirectionItem
          :image="this.imageUrl.english"
          :text="this.textItem.item5"
        />
        <DirectionItem
          :image="this.imageUrl.calligraphy"
          :text="this.textItem.item4"
        />
        <DirectionItem
          :image="this.imageUrl.superMemory"
          :text="this.textItem.item6"
        />
      </div>
    </div>
  </div>
</template>

<script>
import DirectionItem from "./direction/DirectionItem";
import DirectionItemText from "./direction/DirectionItemText";
export default {
  name: "TheDirection",
  components: {
    DirectionItem,
    DirectionItemText,
  },
  data() {
    return {
      text: "Мы развиваем детей с 5 до 16 лет по следующим направлениям",
      imageUrl: {
        mentalArithmetic: require("../assets/icons/mental-arithmetic.png"),
        speedReading: require("../assets/icons/speed-reading.png"),
        preparationForSchool: require("../assets/icons/Preparation-for-school.png"),
        calligraphy: require("../assets/icons/calligraphy.png"),
        english: require("../assets/icons/english.png"),
        superMemory: require("../assets/icons/super-memory.png"),
        afterSchoolClub: require("../assets/icons/after-school-club.png"),
      },
      textItem: {
        item1: "Ментальная арифметика",
        item2: "Скорочтение",
        item3: "Подготовка к школе",
        item4: "Каллиграфия",
        item5: "Английский язык",
        item6: "Супер память",
        item7: "Группа продленного дня ",
      },
    };
  },
};
</script>

<style lang="sass" scoped>
.direction
  padding: 100px 0 60px
  .direction-left
    width: 30%
    margin-top: -15%
    &:nth-child(1)
      // padding-left: 50%

  .direction-center
    display: flex
    flex-direction: column
    margin: 0 auto
    width: 30%
    margin-top: 60px
    img
      max-width: 323px
      max-height: 321px
      margin: 0 auto
      padding: 16px
    p
      padding-bottom: 36px
  .direction-right
    width: 30%
    margin-top: -15%
.direction-left > div:nth-child(1)
  padding-left: 50%
.direction-left > div:nth-child(3)
  padding-left: 50%
.direction-right > div:nth-child(1)
  padding-right: 50%
.direction-right > div:nth-child(3)
  padding-right: 50%
</style>
