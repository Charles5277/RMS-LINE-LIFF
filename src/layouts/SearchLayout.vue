<script setup lang="ts">
import FooterTab from 'src/components/FooterTab.vue';
</script>

<template>
  <q-layout view="lHh Lpr lFf">
    <q-page-container>
      <router-view />
    </q-page-container>

    <FooterTab />
  </q-layout>
</template>

<style lang="scss" scoped>
// header圓角通用class
header {
  border-radius: 0px 0px 35px 35px;
}
</style>
