<script setup lang="ts">

import Header from "~/components/common/Header.vue";
import Footer from "~/components/common/Footer.vue";
</script>

<template>
  <div class="wrap">
    <Header />
      <div class="content">
        <slot></slot>
      </div>
    <Footer />
  </div>
</template>

