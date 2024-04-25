<template>
  <footer class="footer-wrapper text-343741">
    <div class="footer-content">
      <div class="row items-center q-mb-xl">
        <div class="col-md-4 col-12 column">
          <img
            class="q-mb-sm"
            src="/assets/hyperhire-black.png"
            width="187"
            height="34"
          />
          <p class="text-body2 q-mb-sm" style="font-weight: 900">
            우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.
          </p>
          <p class="q-mb-sm" style="font-weight: 900; font-size: 13px">
            010-0000-0000 <br />
            aaaaa@naver.com
          </p>
        </div>
        <div class="col-md-8 col-12 flex items-start q-mt-md-none q-mt-lg">
          <div
            v-for="(item, index) in rightSideFooter"
            :key="index"
            class="card-footer-item q-mr-sm col-12 col-md"
          >
            <q-icon :name="`img:.${item.icon}`" size="40px" />
            <p class="text-body2" style="font-weight: 900">
              {{ item.title }}
            </p>
            <p class="text-body-2 flex items-center" style="font-weight: 600">
              <span class="q-mr-sm">{{ item.subtitle }}</span>
              <span>
                <svg
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M6.59669 2.91675C4.36085 2.91675 2.91669 4.27925 2.91669 6.38758V13.6117C2.91669 15.7201 4.36085 17.0834 6.59669 17.0834H13.4034C15.6392 17.0834 17.0834 15.7201 17.0834 13.6117V6.38758C17.0834 4.27925 15.6392 2.91675 13.4034 2.91675H6.59669ZM13.4034 18.3334H6.59669C3.64835 18.3334 1.66669 16.4359 1.66669 13.6117V6.38758C1.66669 3.56341 3.64835 1.66675 6.59669 1.66675H13.4034C16.3517 1.66675 18.3334 3.56341 18.3334 6.38758V13.6117C18.3334 16.4359 16.3517 18.3334 13.4034 18.3334Z"
                    fill="#5E626F"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M13.4049 10.625H6.59491C6.24991 10.625 5.96991 10.345 5.96991 10C5.96991 9.655 6.24991 9.375 6.59491 9.375H13.4049C13.7499 9.375 14.0299 9.655 14.0299 10C14.0299 10.345 13.7499 10.625 13.4049 10.625Z"
                    fill="#5E626F"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M10.2686 13.7484C10.1086 13.7484 9.94775 13.6876 9.82608 13.5642C9.58275 13.3192 9.58358 12.9242 9.82775 12.6809L12.5194 10.0001L9.82775 7.31925C9.58358 7.07591 9.58275 6.68091 9.82608 6.43591C10.0694 6.19091 10.4644 6.19091 10.7094 6.43425L13.8461 9.55758C13.9644 9.67425 14.0303 9.83425 14.0303 10.0001C14.0303 10.1659 13.9644 10.3259 13.8461 10.4426L10.7094 13.5659C10.5878 13.6876 10.4278 13.7484 10.2686 13.7484Z"
                    fill="#5E626F"
                  />
                </svg>
              </span>
            </p>
          </div>
        </div>
      </div>
      <div class="row items-center q-mb-xl">
        <div class="col-md-4 col-12 flex items-start">
          <div
            v-for="(item, index) in bottomLeftSide"
            :key="index"
            class="column q-pr-lg"
          >
            <p class="text-body2 q-mb-sm" style="font-weight: 900">
              {{ item.title }}
            </p>
            <p class="text-body2 q-mb-sm" style="font-weight: 600">
              {{ item.subtitle }}
            </p>
            <p class="text-body2 q-mb-sm" style="font-weight: 900">
              {{ item.bottom }}
            </p>
          </div>
        </div>
        <div class="col-md-8 col-12 flex items-start q-mt-md-none q-mt-lg">
          <div
            v-for="(item, index) in bottomRightSide"
            :key="index"
            class="column q-pr-lg q-mt-md-none q-mt-sm"
          >
            <p class="text-body2 q-mb-sm" style="font-weight: 900">
              {{ item.title }}
            </p>
            <p class="text-body2 q-mb-sm" style="font-weight: 600">
              {{ item.subtitle }}
            </p>
            <p class="text-body2 q-mb-sm" style="font-weight: 900">
              {{ item.bottom }}
            </p>
          </div>
        </div>
      </div>
      <div class="text-body2" style="font-weight: 900; margin-top: 42px">
        ⓒ 2024 Hyperhire
      </div>
    </div>
  </footer>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
export default defineComponent({
  name: 'MainLayout',
  setup() {
    return {
      rightSideFooter: ref([
        {
          icon: './icons/tag-icon.svg',
          title: '해외 개발자 원격 채용',
          subtitle: '바로가기',
        },
        {
          icon: './icons/tag-user.svg',
          title: '해외 개발자 원격 채용',
          subtitle: '바로가기',
        },
        {
          icon: './icons/tag-kor.svg',
          title: '해외 개발자 원격 채용',
          subtitle: '바로가기',
        },
        {
          icon: './icons/tag-gear.svg',
          title: '해외 개발자 원격 채용',
          subtitle: '바로가기',
        },
      ]),
      bottomLeftSide: ref([
        {
          title: '상호명',
          subtitle: '하이퍼하이어',
          bottom: 'Hyperhire India Private Limited',
        },

        {
          title: '대표 CEO',
          subtitle: '김주현',
          bottom: 'Juhyun Kim',
        },
      ]),
      bottomRightSide: ref([
        {
          title: '사업자등록번호 CIN',
          subtitle: '427-86-01187',
          bottom: 'U74110DL2016PTC290812',
        },

        {
          title: '주소 ADDRESS',
          subtitle: '서울특별시 강남대로 479, 지하 1층 238호',
          bottom:
            'D-138, Street number 11, Jagjeet Nagar, North East Delhi, New Delhi, 110053 India',
        },
      ]),
    };
  },
});
</script>

<style lang="scss" scoped>
.footer-wrapper {
  background: #fbfbfb;
  min-height: 505px;
  width: 100vw;
  padding: 16px;
  .footer-content {
    margin: 42px auto;
    max-width: 1280px;
  }
  .card-footer-item {
    background-color: white;
    border-radius: 12px;
    padding: 16px;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }
}
</style>
