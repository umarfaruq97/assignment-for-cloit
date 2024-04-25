<template>
  <div
    data-aos="zoom-in-left"
    data-aos-duration="600"
    data-aos-delay="300"
    data-aos-mirror="true"
    class="home-carousel-wrapper"
  >
    <div
      class=""
      style="position: relative; width: fit-content; margin: 16px auto"
    >
      <div
        class="text-40e2e8 bg-white flex items-center"
        style="
          font-size: 18px;
          width: fit-content;
          padding: 6px 12px;
          border-radius: 8px;
          gap: 8px;
        "
      >
        <svg
          width="27"
          height="27"
          viewBox="0 0 27 27"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="13.7607" cy="13.5" r="13" fill="#BBF3D2"></circle>
          <path
            d="M17.9441 9.60332C17.3592 9.60332 16.9024 9.13165 16.5905 8.63687C16.5455 8.56539 16.496 8.49643 16.442 8.42998C16.1812 8.10063 15.8279 7.85361 15.3819 7.68893C14.9358 7.52426 14.4281 7.44192 13.8586 7.44192C13.2616 7.44192 12.7367 7.53455 12.2838 7.71981C11.831 7.90507 11.481 8.16581 11.234 8.50203C10.987 8.83139 10.8635 9.20877 10.8635 9.63419C10.8635 10.2655 11.1208 10.7526 11.6354 11.0957C12.1569 11.4319 12.8053 11.6927 13.5807 11.8779L15.0113 12.2587C16.2533 12.5675 17.2791 13.041 18.0887 13.6791C18.9053 14.3172 19.3135 15.247 19.3135 16.4683C19.3135 17.3123 19.094 18.0671 18.6548 18.7326C18.2225 19.3914 17.5878 19.906 16.7507 20.2765C15.9205 20.647 14.9324 20.8323 13.7865 20.8323C12.675 20.8323 11.7109 20.6539 10.8944 20.2971C10.0847 19.9403 9.44658 19.436 8.98 18.7841C8.7372 18.4398 8.55086 18.0611 8.42099 17.648C8.22397 17.0212 8.76291 16.458 9.41988 16.458C10.0143 16.458 10.4742 16.9427 10.7681 17.4593C10.8313 17.5704 10.9042 17.6757 10.987 17.7755C11.2889 18.1323 11.68 18.3999 12.1603 18.5783C12.6475 18.7567 13.1861 18.8424 13.7762 18.8356C14.4075 18.8356 14.9736 18.7361 15.4745 18.5371C15.9754 18.3381 16.3665 18.0568 16.6478 17.6931C16.9291 17.3295 17.0698 16.9075 17.0698 16.4272C17.0698 16.0155 16.9532 15.6655 16.7199 15.3773C16.4866 15.0891 16.1675 14.8559 15.7627 14.6775C15.3578 14.4991 14.8569 14.3309 14.26 14.1731L12.4897 13.71C11.2409 13.3669 10.2803 12.8763 9.60783 12.2382C8.94226 11.5932 8.6129 10.7664 8.61976 9.7577C8.61976 8.91373 8.8462 8.16581 9.29906 7.51396C9.75879 6.86211 10.3901 6.36122 11.1929 6.01128C12.0025 5.65448 12.9083 5.47607 13.91 5.47607C14.905 5.47607 15.7935 5.65448 16.5758 6.01128C17.3648 6.36122 17.979 6.85182 18.4181 7.48309C18.6365 7.78891 18.8031 8.11449 18.9179 8.45983C19.1195 9.06655 18.5834 9.60332 17.9441 9.60332Z"
            fill="#00C696"
          ></path>
          <path
            d="M13.9512 4.5L13.9512 6.3291"
            stroke="#00C696"
            stroke-width="2"
            stroke-linecap="round"
          ></path>
          <path
            d="M13.9512 19.918L13.9512 21.7471"
            stroke="#00C696"
            stroke-width="2"
            stroke-linecap="round"
          ></path>
        </svg>
        월 100만원
      </div>
      <svg
        width="12"
        height="11"
        viewBox="0 0 12 11"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        style="position: absolute; bottom: -9px; left: 50%; color: white"
      >
        <path
          d="M6.43301 10.25C6.24056 10.5833 5.75944 10.5833 5.56699 10.25L0.370835 1.25C0.178386 0.916665 0.418948 0.499999 0.803848 0.499999L11.1962 0.5C11.5811 0.5 11.8216 0.916667 11.6292 1.25L6.43301 10.25Z"
          fill="currentColor"
        ></path>
      </svg>
    </div>
    <Carousel :itemsToShow="2" :wrapAround="true" :transition="500">
      <Slide v-for="slide in 10" :key="slide">
        <div class="home-carousel__item">
          <div class="column items-center" style="gap: 16px">
            <div style="position: relative">
              <div class="q-avatar" style="font-size: 120px">
                <div class="q-avatar__content row flex-center overflow-hidden">
                  <img src="/assets/avatar.f5767347.png" />
                </div>
              </div>
              <img
                src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABkAAAASCAYAAACuLnWgAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAACPSURBVHgB7ZUxCsJgDIW/hB6gIt0d6nW8gmfwBOoNPJnoLthdkH8W6tMiVBHEpSki/aaEPHghb4hpX8xrsRGe0zGOKjetrN4VR8GEOJIHGzTkTg8MJr9nkoHaxnh2r/W3GW+6K4/tW305W37Sd0Z2OI2J5o+CLy9norHtaBoefG+ZJGJpfgqL+9UqYkgS6xt2UiXTpL5DFAAAAABJRU5ErkJggg=="
                style="position: absolute; bottom: 0px; right: 14px"
              />
            </div>
            <div class="column items-center">
              <div class="text-24252f" style="font-size: 24px">
                Abhishek Gupta
              </div>
              <div class="text-4a77ff" style="font-size: 16px">
                마케팅 · 2y+
              </div>
            </div>
          </div>
          <div class="text-5e626f column" style="gap: 4px; font-size: 16px">
            <div class="column items-center" style="gap: 4px; color: #5e626f">
              <div
                class="q-py-xs q-px-sm"
                style="
                  border: solid;
                  width: fit-content;
                  border-radius: 6px;
                  border-color: #c1c5cf;
                "
              >
                마케팅 콘텐츠 제작
              </div>
              <div
                class="q-py-xs q-px-sm"
                style="
                  border: solid;
                  width: fit-content;
                  border-radius: 6px;
                  border-color: #c1c5cf;
                "
              >
                인스타그램 관리
              </div>
            </div>
            <div class="row justify-center" style="gap: 4px">
              <div
                class="q-py-xs q-px-sm"
                style="
                  border: solid;
                  width: fit-content;
                  border-radius: 6px;
                  border-color: #c1c5cf;
                "
              >
                트위터 관리
              </div>
              <div
                class="q-py-xs q-px-sm"
                style="
                  border: solid;
                  width: fit-content;
                  border-radius: 6px;
                  border-color: #c1c5cf;
                "
              >
                블로그 글 작성
              </div>
            </div>
          </div>
        </div>
      </Slide>
      <template #addons>
        <Navigation />
      </template>
      ...
    </Carousel>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import { Carousel, Slide, Navigation } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';

export default defineComponent({
  name: 'HomeCarousel',
  components: {
    Carousel,
    Slide,
    Navigation,
  },
});
</script>

<style lang="scss">
.home-carousel-wrapper {
  .carousel__slide {
    padding: 5px;
  }

  .carousel__viewport {
    perspective: 2000px;
  }

  .carousel__track {
    transform-style: preserve-3d;
    min-height: 464px;
  }

  .carousel__slide--sliding {
    transition: 0.5s;
  }

  .carousel__slide {
    opacity: 0.9;
    transform: rotateY(-20deg) scale(0.9);
  }

  .carousel__slide--active ~ .carousel__slide {
    transform: rotateY(20deg) scale(0.9);
  }

  .carousel__slide--prev {
    opacity: 1;
    transform: rotateY(-10deg) scale(0.95);
  }

  .carousel__slide--next {
    opacity: 1;
    transform: rotateY(10deg) scale(0.95);
  }

  .carousel__slide--active {
    opacity: 1;
    transform: rotateY(0) scale(1.1);
  }
  .home-carousel__item {
    width: 292px;
    min-height: 408px;
    background-color: white;
    color: #fff;
    font-size: 20px;
    border-radius: 8px;
    display: flex;
    flex-direction: column;
    padding: 24px;
    border-radius: 12px;
    gap: 24px;
    box-shadow: rgba(0, 0, 0, 0.12) 0px 15px 24px 0px;
  }
}
</style>
