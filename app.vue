<script setup>

const isDarkMode = ref(false);
const title = "Spaces | Home";
</script>
<template>
  <div :class="{ dark: isDarkMode }">
    <Head>
      <Title>{{ title }}</Title>
      <Meta name="description" :content="title" />
    </Head>
    <main class="min-h-svh dark:bg-gray-950 dark:text-gray-50">
      <div
        class="grid grid-cols-12 mx-auto md:px-6 lg:max-w-7xl lg:px-8 lg:gap-5"
      >
        <!-- left sidebar -->
        <div class="hidden sm:block col-span-1 xl:col-span-2">
          <SidebarLeft />
        </div>
        <!-- main content -->
         <div class="col-span-12 md:col-span-8
         xl:col-span-6"
         </div>
         <!-- right sidebar -->
          <div class="hidden sm:block md:col-span-3 xl:col-span-3">
            <SidebarRight />
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
