<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<script setup lang="ts">
useHead({
  titleTemplate: (title = '') => title + (title && ' - ') + 'PKU Mirrors'
})
</script>
