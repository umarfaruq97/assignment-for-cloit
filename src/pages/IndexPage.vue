<template>
  <q-page class="column full-width justify-center">
    <div class="row items-center justify-between full-width q-pt-lg">
      <div
        class="col-md-6 col-12 q-px-sm col-grow flex column justify-md-start justify-center text-white"
      >
        <div
          data-aos="fade-left"
          data-aos-duration="600"
          data-aos-delay="900"
          class="relative-position q-mb-md"
        >
          <div
            :class="`text-h6 ${
              $q.screen.gt.sm ? 'text-40e2e8 bg-white' : 'text-white bg-8bb4ff'
            }`"
            style="width: fit-content; padding: 6px 12px; border-radius: 8px"
          >
            풀타임, 파트타임
          </div>
          <svg
            width="12"
            height="11"
            viewBox="0 0 12 11"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            :style="{
              position: 'absolute',
              bottom: '-9px',
              left: '9px',
              color: $q.screen.gt.sm ? 'white' : '#8bb4ff',
            }"
          >
            <path
              d="M6.43301 10.25C6.24056 10.5833 5.75944 10.5833 5.56699 10.25L0.370835 1.25C0.178386 0.916665 0.418948 0.499999 0.803848 0.499999L11.1962 0.5C11.5811 0.5 11.8216 0.916667 11.6292 1.25L6.43301 10.25Z"
              fill="currentColor"
            ></path>
          </svg>
        </div>
        <div data-aos="fade-up" data-aos-duration="500" class="text-h3">
          최고의 실력을 가진<br />
          외국인 인재를 찾고 계신가요?
        </div>
        <div
          data-aos="fade-down"
          data-aos-duration="500"
          key="h5-title"
          class="text-h5"
        >
          법률 및 인사관리 부담없이<br />
          1주일 이내에 원격으로 채용해보세요.
        </div>
        <div v-if="$q.screen.gt.sm" key="h6-subtitle" class="text-h6">
          개발자가 필요하신가요?
        </div>
        <div
          v-if="$q.screen.gt.sm"
          data-aos="fade-left"
          data-aos-duration="500"
          data-aos-mirror="true"
          key="flex-line"
          class="row items-start"
          style="gap: 48px"
        >
          <div
            class="q-pt-sm q-mr-sm"
            style="
              gap: 8px;
              border-top: 1px solid white;
              border-right-color: white;
              border-bottom-color: white;
              border-left-color: white;
            "
          >
            <div class="text-h6">평균 월 120만원</div>
            <div class="text-body1">
              임금을 해당 국가를 기준으로 계산합니다.
            </div>
          </div>
          <div
            class="q-pt-sm q-mr-sm"
            style="
              gap: 8px;
              border-top: 1px solid white;
              border-right-color: white;
              border-bottom-color: white;
              border-left-color: white;
            "
          >
            <div class="text-h6">평균 월 120만원</div>
            <div class="text-body1">
              임금을 해당 국가를 기준으로 계산합니다.
            </div>
          </div>
          <div
            class="q-pt-sm q-mr-sm"
            style="
              gap: 8px;
              border-top: 1px solid white;
              border-right-color: white;
              border-bottom-color: white;
              border-left-color: white;
            "
          >
            <div class="text-h6">평균 월 120만원</div>
            <div class="text-body1">
              임금을 해당 국가를 기준으로 계산합니다.
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6 col-12 q-px-sm col-grow">
        <HomeCarousel />
      </div>
    </div>
    <div class="full-width q-mt-lg q-pt-lg">
      <BottomCarousel />
    </div>
  </q-page>
</template>

<script>
import HomeCarousel from '../components/HomeCarousel.vue';
import BottomCarousel from '../components/BottomCarousel.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'IndexPage',
  components: {
    HomeCarousel,
    BottomCarousel,
  },
});
</script>

<style lang="scss"></style>
