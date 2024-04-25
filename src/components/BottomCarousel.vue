<template>
  <div class="bottom-carousel-wrapper">
    <Carousel
      v-if="!$q.screen.lt.sm"
      v-bind="settings"
      :breakpoints="breakpoints"
    >
      <Slide v-for="slide in slideItems" :key="slide">
        <div class="carousel__item">
          <div class="icon-wrapper q-mr-md">
            <q-icon :name="`img:.${slide.icon}`" size="32px" :color="'#FFF'" />
          </div>
          <div class="text-wrapper">
            {{ slide.text }}
          </div>
        </div>
      </Slide>
    </Carousel>
    <div v-else class="column">
      <div class="row q-px-md">
        <div
          v-for="(item, index) in checkboxList"
          :key="index"
          class="col-5 flex items-center"
        >
          <div class="q-py-sm q-pr-sm">
            <q-icon name="img:./icons/checkbox.svg" size="20px" />
          </div>
          <span class="text-body1 text-white q-py-sm" style="font-weight: 900">
            {{ item }}
          </span>
        </div>
      </div>
      <div
        class="text-body1 q-pa-md"
        style="font-weight: 900; color: #fbff23; text-decoration: underline"
      >
        개발자가 필요하신가요?
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import { Carousel, Slide } from 'vue3-carousel';

import 'vue3-carousel/dist/carousel.css';

export default defineComponent({
  name: 'BottomCarousel',
  components: {
    Carousel,
    Slide,
  },
  data: () => ({
    // carousel settings
    settings: {
      itemsToShow: 1.5,
      autoplay: 5000,
      wrapAround: true,
      snapAlign: 'center',
    },
    // breakpoints are mobile first
    // any settings not specified will fallback to the carousel settings
    breakpoints: {
      // 700px and up
      700: {
        itemsToShow: 2.5,
        autoplay: 5000,
        wrapAround: true,
        snapAlign: 'center',
      },
      // 1024 and up
      1024: {
        itemsToShow: 4,
        autoplay: 5000,
        wrapAround: true,
        snapAlign: 'start',
      },
      1200: {
        itemsToShow: 4.5,
        autoplay: 5000,
        wrapAround: true,
        snapAlign: 'start',
      },
    },
    slideItems: [
      {
        icon: './icons/icon-marketing.svg',
        text: '해외 마케팅',
      },
      {
        icon: './icons/icon-image.svg',
        text: '퍼블리셔',
      },
      {
        icon: './icons/icon-box.svg',
        text: '캐드원(제도사)',
      },
      {
        icon: './icons/icon-target.svg',
        text: '해외 세일즈',
      },
      {
        icon: './icons/icon-call.svg',
        text: '퍼블리셔',
      },
    ],
    checkboxList: ['한국어 능력', '업무 수행 능력', '겸업 여부', '평판 조회'],
  }),
});
</script>

<style lang="scss">
.bottom-carousel-wrapper {
  .carousel__item {
    margin: 0 8px;
    padding: 16px;
    border-radius: 12px;
    display: flex;
    align-items: center;
    width: 100%;
    background-color: rgba(255, 255, 255, 0.2);
    .icon-wrapper {
      display: flex;
      padding: 12px;
      border-radius: 8px;
      align-items: center;
      justify-content: center;
      background-color: rgba(255, 255, 255, 0.2);
    }
    .text-wrapper {
      font-size: 24px;
      line-height: 36px;
      font-weight: 900;
      color: white;
      margin-right: 12px;
    }
  }
}
</style>
