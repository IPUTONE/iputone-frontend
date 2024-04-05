<script setup lang="ts">
useHead({
  meta: [
    { charset: 'utf-8' },
    { name: 'viewport', content: 'width=device-width,initial-scale=1' },
  ],
  link: [
    {
      href: 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css',
      rel: 'stylesheet',
    },
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
