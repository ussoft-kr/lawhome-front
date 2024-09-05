<script setup lang="ts">

import Header from "~/components/common/Header.vue";
import Footer from "~/components/common/Footer.vue";
import { useHead } from "#app";

useHead({
  title : '법률구조법인 한국가정법률상담소',
  meta : [
    {name : 'description', content: '한국가정법률상담소 페이지입니다.'},
    {name : 'keywords', content : '한국가정법률상담소에서 법률상담을 받아보세요'},
    {name : 'viewport',content: 'width=device-width, initial-scale=1'}
  ]
})


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

