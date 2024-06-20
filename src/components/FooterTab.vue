<script setup lang="ts">
import { ref } from 'vue';
const tab = ref('home');
</script>

<template>
  <q-footer class="q-px-md" style="background-color: transparent">
    <q-tabs
      v-model="tab"
      class="bg-white text-grey-7 shadow-2 row full-width justify-center q-mb-md"
      indicator-color="blue-7"
      active-color="blue-7"
      inline-label
      switch-indicator
      style="
        border: 1px solid rgba(29, 24, 242, 0.2);
        border-radius: 0px 0px 10px 10px;
        box-shadow:
          -10px 0 10px 3px rgba(79, 74, 242, 0.2),
          10px 0 10px 3px rgba(79, 74, 242, 0.2),
          0 10px 5px 3px rgba(200, 210, 230, 0.1),
          0 -10px 5px 3px rgba(200, 210, 230, 0.1);
      "
    >
      <q-route-tab
        name="home"
        icon="home"
        class="q-pa-none"
        :to="{ name: 'home' }"
        :ripple="false"
        exact
        no-caps
        style="min-width: 90px; flex-grow: 1"
      />
      <q-route-tab
        name="search"
        icon="search"
        class="q-pa-none"
        :to="{ name: 'search' }"
        :ripple="false"
        exact
        no-caps
        style="min-width: 90px; flex-grow: 1"
      />
    </q-tabs>
  </q-footer>
</template>
