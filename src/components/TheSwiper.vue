<template>
  <div>
    <div>
      <h2 class="text-2xl">Слайдер</h2>
    </div>
    <div class="slider-block border border-yellow-400 mt-10 h-">
      <swiper
        :slidesPerView="3"
        :spaceBetween="30"
        :slidesPerGroup="3"
        :loop="true"
        :loopFillGroupWithBlank="true"
        :pagination="{
          clickable: true,
        }"
        :navigation="true"
        class="mySwiper w-1/4"
      >
        <swiper-slide v-for="(item, index) in 9" :key="index"
          >Slide 1</swiper-slide
        >
      </swiper>
    </div>
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
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
};
</script>
