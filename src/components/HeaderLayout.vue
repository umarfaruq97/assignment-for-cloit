<template>
  <q-header elevated class="bg-transparent shadow-0" reveal>
    <q-toolbar class="toolbar-wrapper">
      <img
        alt="Hyperhire Logo"
        src="data:image/png;base64,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"
        style="width: 114px; height: 21px"
      />
      <template v-if="!$q.screen.lt.sm">
        <div class="flex items-center">
          <q-btn-dropdown
            color="primary"
            label="채용"
            class="bg-transparent"
            dropdown-icon="fa-solid fa-chevron-down"
            unelevated
            no-caps
          >
            <q-list style="min-width: 100px">
              <q-item>
                <q-item-section>
                  <q-item-label>채용</q-item-label>
                </q-item-section>
              </q-item>

              <q-item>
                <q-item-section>
                  <q-item-label>해외 개발자 원격 채용</q-item-label>
                </q-item-section>
              </q-item>

              <q-item>
                <q-item-section>
                  <q-item-label>외국인 원격 채용 (비개발 직군)</q-item-label>
                </q-item-section>
              </q-item>
              <q-item>
                <q-item-section>
                  <q-item-label>한국어 가능 외국인 채용</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-btn-dropdown>
          <div class="q-ml-lg q-px-lg cursor-pointer non-selectable">
            해외 개발자 활용 서비스
          </div>
        </div>
        <q-btn
          unelevated
          no-caps
          style="
            background-color: white;
            color: rgb(74, 119, 255);
            border-radius: 8px;
            padding: 6px 24px;
          "
        >
          문의하기
        </q-btn>
      </template>
    </q-toolbar>
  </q-header>
</template>

<script>
export default {};
</script>

<style lang="scss">
.q-header .q-layout__shadow:after {
  box-shadow: none;
}
.toolbar-wrapper {
  margin: auto;
  min-height: 50px;
  display: flex;
  align-items: center;
  justify-content: space-around;
  .q-btn--actionable.q-btn--standard:active:before,
  .q-btn--actionable.q-btn--standard.q-btn--active:before {
    box-shadow: none;
  }
  .q-btn .q-icon {
    font-size: 12px !important;
  }
}
@media screen and (max-width: 600px) {
  .toolbar-wrapper {
    justify-content: start;
    margin: 0;
  }
}
</style>
