/* eslint-disable */
<template>
  <div id="catalog" class="catalog">
    <TheTitle title="Каталог" />
    <!-- <div class="container"> -->
    <div class="img-left"></div>
    <div class="img-right"></div>
    <swiper
      :slidesPerView="3"
      :spaceBetween="-50"
      :slidesPerGroup="1"
      :loop="true"
      :loopFillGroupWithBlank="true"
      :navigation="true"
      class="mySwiper w-1/4"
    >
      <swiper-slide>
        <CatalogItem
          itemHeadTitle="Подготовка к школе"
          itemTitle="30 000  тг"
          color="#018FA3"
          numArr="0"
        />
      </swiper-slide>
      <swiper-slide>
        <CatalogItem
          itemHeadTitle="скорочтение"
          itemTitle="27 000  тг"
          color="#955EEA"
          numArr="1"
        />
      </swiper-slide>
      <swiper-slide>
        <CatalogItem
          itemHeadTitle="ментальная арифметика"
          itemTitle="20 000  тг"
          color="#4ECA30"
          numArr="2"
        />
      </swiper-slide>
      <swiper-slide>
        <CatalogItem
          itemHeadTitle="Каллиграфия"
          itemTitle="24 000  тг"
          color="#FFE41B"
          numArr="3"
        />
      </swiper-slide>
      <swiper-slide>
        <CatalogItem
          itemHeadTitle="Английский язык"
          itemTitle="18 000  тг"
          color="#FF4D94"
          numArr="4"
        />
      </swiper-slide>
      <swiper-slide>
        <CatalogItem
          itemHeadTitle="Группа продленного дня"
          itemTitle="35 000  тг"
          color="#FFA724"
          numArr="5"
        />
      </swiper-slide>
    </swiper>
    <!-- </div> -->
  </div>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// swiper bundle styles
// import "swiper/swiper-bundle.min.css";

// swiper core styles
// import "swiper/swiper.min.css";

// modules styles
import "swiper/components/navigation/navigation.min.css";
import "swiper/components/pagination/pagination.min.css";

// import Swiper core and required modules
import SwiperCore, { Pagination, Navigation } from "swiper";

// install Swiper modules
SwiperCore.use([Pagination, Navigation]);

import TheTitle from "./TheTitle.vue";
import CatalogItem from "./catalog/CatalogItem";
export default {
  name: "TheCatalog",
  components: {
    TheTitle,
    CatalogItem,
    Swiper,
    SwiperSlide,
  },
  data() {
    return {};
  },
};
</script>

<style lang="sass">
.catalog
  background: #F6FAFF
  padding-bottom: 100px
  position: relative
  z-index: 1
  .img-left
    width: 200px
    height: 200px
    position: absolute
    border-radius: 10em
    background: #FFF7BE
    left: 0
    top: 21%
  .img-right
    position: absolute
    width: 150px
    height: 180px
    right: 160px
    top: 16%
    border: 13px solid #089EA5
    border-radius: 10em
  .title
    padding-top: 70px
.swiper-button-next, .swiper-button-prev
  color: #000
.swiper-slide .swiper-slide-active
  width: 387px !important
</style>
