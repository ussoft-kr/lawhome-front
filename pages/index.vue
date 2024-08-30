<script setup lang="ts">
  import { ref } from "vue";
  import { useFetch } from "#app";

  const { data } = await useFetch('/api/test/hello');

  const message = ref(data.value.message);

</script>

<template>
  <v-container>
    <h1 class="text-center">Nuxt.js + Vuetify Welcome</h1>
    <p class="text-center">{{message}}</p>
  </v-container>
</template>

