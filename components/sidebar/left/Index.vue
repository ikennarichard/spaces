<template>
  <aside class="flex flex-col h-screen gap-4">
    <nuxt-link to="/" class="p-2">
      <Logo />
    </nuxt-link>
    <SidebarLeftTab>
      <template v-slot:icon>
        <HomeIcon />
      </template>
      <template v-slot:title>
        Home
      </template>
    </SidebarLeftTab>
  </aside>
</template>

<script setup>
import { HomeIcon } from '@heroicons/vue/24/solid'
</script>