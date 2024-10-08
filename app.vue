<script setup>
const isDarkMode = ref(false);
</script>
<template>
  <div :class="{ dark: isDarkMode }">
    <main class="min-h-svh dark:bg-gray-950 dark:text-gray-50">
      <div class="grid grid-cols-12 mx-auto md:px-6 lg:max-w-7xl lg:px-8 lg:gap-5">
        <!-- left sidebar -->
        <div class="md:block col-span-1 xl:col-span-2">
          <SidebarLeft />
        </div>
      </div>
    </main>
  </div>
</template>

<style>
  body {
    font-family: "Inter", sans-serif;
  }
</style>
