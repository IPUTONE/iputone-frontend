<script setup lang="ts">
const baseUrl = 'https://iput-one.com';
const endpoint = baseUrl + '/wp-json/wp/v2/posts/1';
const data = await useFetch(endpoint);
console.log(data);
</script>

<template></template>
