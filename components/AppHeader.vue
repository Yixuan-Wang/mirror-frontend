<template>
  <header class="flex items-center px-8 gap-2 backdrop-filter backdrop-blur">
    <div>
      <img :src="pku" class="h-12" />
    </div>
    <div>
      <img :src="mirror" class="h-8 mt-2" />
    </div>
    <div class="flex-1"></div>
    <NuxtLink
      v-for="(link, i) of links"
      :key="i"
      :to="link.to"
      class="self-stretch flex items-center px-4 hover:bg-#700e0d0a transition"
    >
      {{ link.text }}
    </NuxtLink>
  </header>
</template>

<script setup lang="ts">
import pku from '@/assets/images/pku.svg'
import mirror from '@/assets/images/mirror-text.svg'

const links = [
  { to: '/', text: 'Mirrors' },
  { to: '/help', text: 'Help' },
  { to: '/status', text: 'Status' }
]
</script>
