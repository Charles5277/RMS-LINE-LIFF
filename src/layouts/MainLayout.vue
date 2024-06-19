<script setup lang="ts">
import { ref } from 'vue';

const text = ref('');
</script>

<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar class="q-pl-xl q-pt-lg q-pr-lg" style="height: 80px">
        <q-toolbar-title style="color: rgba(0, 0, 0, 73)">
          歡迎使用資彙王
        </q-toolbar-title>
        <div style="width: 72px">
          <q-avatar size="xl" color="grey-6" text-color="white">
            <img src="https://cdn.quasar.dev/img/boy-avatar.png" />
          </q-avatar>
        </div>
      </q-toolbar>
      <div
        class="full-width row justify-center"
        style="height: 70px; position: relative; top: 40px"
      >
        <q-input
          v-model="text"
          label="您想搜尋什麼？"
          outlined
          rounded
          bg-color="white"
          class="full-width"
          style="padding: 0px 50px; z-index: 100000"
        >
          <template #prepend>
            <q-icon name="search" />
          </template>
        </q-input>
      </div>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<style lang="scss" scoped>
// header圓角通用class
header {
  border-radius: 0px 0px 35px 35px;
}
</style>
