<script setup>
const { spaceBorderColor } = useTransition();
const props = defineProps({
  title: String,
  required: true,
});
</script>

<template>
  <div
    class="m-2 border border-gray-50 overflow-hidden"
    :class="spaceBorderColor"
  >
    <h1 class="p-3 text-xl font-extrabold text-gray-900 border-b dark:text-gray-50">
      {{ props.title }}
    </h1>
    <slot></slot>
    <div class="p-3 text-sm text-gray-800 cursor-pointer hover:bg-gray-100 dark:text-gray-50 dark:hover:bg-gray-900">
      Show more
    </div>
  </div>
</template>
