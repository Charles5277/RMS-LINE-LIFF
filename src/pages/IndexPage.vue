<script setup lang="ts">
// import { ref } from 'vue';
</script>

<template>
  <q-page class="q-py-xl">
    <div class="row justify-center q-gutter-sm">
      <q-intersection v-for="index in 60" :key="index" class="example-item">
        <q-card flat bordered class="q-ma-sm">
          <img src="https://cdn.quasar.dev/img/mountains.jpg" />

          <q-card-section>
            <div class="text-h6">Card #{{ index }}</div>
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
