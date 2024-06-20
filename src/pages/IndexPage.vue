<script setup lang="ts">
import { ref } from 'vue';
const data = ref([
  {
    name: '人物',
    icon: 'mdi-account',
  },
  {
    name: '搜尋',
    icon: 'search',
  },
  {
    name: '動漫',
    icon: 'sym_o_manga',
  },
  {
    name: '動物',
    icon: 'sym_o_pets',
  },
  {
    name: '曲線圖',
    icon: 'sym_o_monitoring',
  },
  {
    name: '餐廳',
    icon: 'sym_o_restaurant',
  },
  {
    name: '地點',
    icon: 'sym_o_location_on',
  },
  {
    name: '書籍',
    icon: 'sym_o_import_contacts',
  },
]);
</script>

<template>
  <q-page class="q-py-xl">
    <div class="row justify-center q-gutter-sm">
      <q-intersection
        v-for="(item, index) in data"
        :key="index"
        class="example-item"
      >
        <q-card
          flat
          bordered
          class="q-ma-sm row justify-center"
          style="border-radius: 20px"
        >
          <!-- <img src="https://cdn.quasar.dev/img/mountains.jpg" /> -->
          <q-icon :name="item.icon" size="60px" class="q-mt-md" />

          <q-card-section class="full-width row justify-center">
            <div class="text-h6">{{ item.name }}</div>
          </q-card-section>
        </q-card>
      </q-intersection>
    </div>
  </q-page>
</template>

<style lang="scss" scoped>
.example-item {
  height: 170px;
  width: 170px;
}
</style>
