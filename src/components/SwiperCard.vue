<template>
  <swiper :effect="'cards'" :grabCursor="true" :modules="modules" class="mySwiper">
    <swiper-slide>
      <h2>①48÷6</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>答え：8</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>②3×8</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>答え：24</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>③10+6</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>答え：16</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>④12-8</h2>
    </swiper-slide>
    <swiper-slide>
      <h2>答え：4</h2>
    </swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/effect-cards';

import './style.css';

// import required modules
import { EffectCards } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectCards],
    };
  },
};
</script>
