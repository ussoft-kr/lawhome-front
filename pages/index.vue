<script setup lang="ts">
  import { ref } from "vue";
  import { useFetch } from "#app";
  import '@styles/main.css';
  const { data } = await useFetch('/api/test/hello');
  const message = ref (data.value.message);


</script>

<template>
  <v-container>
    <h1 class="text-center">메인!</h1>
    <p class="text-center">api 테스트! 메세지는 {{message}}</p>
  </v-container>
</template>
