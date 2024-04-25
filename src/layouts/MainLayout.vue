<template>
  <q-layout view="lHh Lpr lFf" class="shadow-0">
    <HeaderLayout />
    <q-page-container class="page-container">
      <div class="content-wrapper">
        <router-view />
      </div>
    </q-page-container>
    <FooterLayout />
  </q-layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import FooterLayout from '../components/FooterLayout.vue';
import HeaderLayout from '../components/HeaderLayout.vue';
export default defineComponent({
  name: 'MainLayout',
  components: {
    FooterLayout,
    HeaderLayout,
  },
});
</script>

<style lang="scss">
.page-container {
  min-height: 717px;
  padding: 122px 0px;
  overflow: hidden;
  background: linear-gradient(151.17deg, #26c2b9 8.69%, #288be7 126.06%);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-blend-mode: color-burn;
}
.content-wrapper {
  max-width: 1280px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-around;
}
</style>
