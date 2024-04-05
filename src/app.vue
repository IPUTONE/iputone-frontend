<script setup lang="ts">
useHead({
  meta: [
    { charset: 'utf-8' },
    { name: 'viewport', content: 'width=device-width,initial-scale=1' },
  ],
});

useSeoMeta({
  title: 'IPUT ONE',
  ogTitle: 'IPUT ONE',
  description: 'IPUT ONE 国際工科専門職大学サークルサイト',
  ogDescription: 'IPUT ONE 国際工科専門職大学サークルサイト',
  ogImage: '',
  twitterCard: 'summary_large_image',
});
</script>

<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
