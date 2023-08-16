<template>
  <div class="reviews" id="reviews">
    <TheTitle title="Отзывы" />
    <!-- <div class="container"> -->
    <swiper
      :slidesPerView="3"
      :spaceBetween="-30"
      :slidesPerGroup="1"
      :loop="true"
      :loopFillGroupWithBlank="true"
      :navigation="true"
      class="mySwiper w-1/4"
    >
      <swiper-slide>
        <ReviewsItem
          :image="imagesReviews.malika"
          itemText="Искренне рекомендую, детям дают отличные знания и безопасность. Профессионалы своего дела. Удачи вам и успехов желаю."
          name="Malika Fazlieva"
        />
      </swiper-slide>
      <swiper-slide>
        <ReviewsItem
          :image="imagesReviews.aigul"
          itemText="Отлично все нравится! Внучка уже 6 месяц занимается, довольны"
          name="Aigul Lepessova"
        />
      </swiper-slide>
      <swiper-slide>
        <ReviewsItem
          :image="imagesReviews.malika2"
          itemText="Маған ұнаған жері білімді жақсы береді. Ұлымның қатынап жүргеніне 1 ай болмады бірақ нәтиже бар. Мұғалімдеріде өте сыпайы әрі білімді."
          name="Malika Fazlieva"
        />
      </swiper-slide>
      <swiper-slide>
        <ReviewsItem
          :image="imagesReviews.anara"
          itemText="Искренне рекомендую, детям дают отличные знания и безопасность. Профессионалы своего дела. Удачи вам и успехов желаю."
          name="Анара Баймаганбетова"
        />
      </swiper-slide>
      <swiper-slide>
        <ReviewsItem
          :image="imagesReviews.gulzhan"
          itemText="Комфорная обстановака, распологает к учебе, учителя доброжелательные,но требовательные! То, что надо! Советую 100%."
          name="Gulzhan Kossantayeva"
        />
      </swiper-slide>
      <swiper-slide>
        <ReviewsItem
          :image="imagesReviews.enlik"
          itemText="Айжан Талгатовна өз ісінің маманы. Менің қызымның оқу үлгеріміне көп ықпал тигіздіңіз. Кемеңгер мектебі нағыз кеменгер бала тәлімін береді!"
          name="Енлик Серик"
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
import "swiper/swiper-bundle.min.css";

// swiper core styles
import "swiper/swiper.min.css";

// modules styles
import "swiper/components/navigation/navigation.min.css";
import "swiper/components/pagination/pagination.min.css";

// import Swiper core and required modules
import SwiperCore, { Pagination, Navigation } from "swiper";

// install Swiper modules
SwiperCore.use([Pagination, Navigation]);
import TheTitle from "./TheTitle.vue";
import ReviewsItem from "./reviews/ReviewsItem.vue";
export default {
  name: "TheReviews",
  components: {
    TheTitle,
    ReviewsItem,
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      imagesReviews: {
        malika: require("../assets/malika.png"),
        aigul: require("../assets/aigul.png"),
        malika2: require("../assets/malika2.png"),
        anara: require("../assets/anara.png"),
        gulzhan: require("../assets/gulzhan.png"),
        enlik: require("../assets/enlik.png"),
      },
    };
  },
};
</script>

<style lang="sass">
.left
  left: -30px
.reviews
  padding-bottom: 60px
  .container
    position: relative
    // width: 1350px !important
.swiper-slide
  // width: 407px !important
</style>
