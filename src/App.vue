<template>
  <SpeedInsights />
  <v-app>
    <app-header />
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts" setup>
import AppHeader from './components/AppHeader.vue';
import { SpeedInsights } from "@vercel/speed-insights/vue"

  //
</script>
