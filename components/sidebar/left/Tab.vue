<template>
  <nuxt-link
    to="#"
    class="flex items-center p-2 rounded-full w-min hover:bg-gray-200 dark:hover:bg-gry-200"
  >
    <span class="inline-block w-6 h-6 text-dark">
      <slot name="icon"></slot>
    </span>
    <span class="ml-4 text-xl" :class="textActive">
      <slot name="title"></slot>
    </span>
  </nuxt-link>
</template>

<script setup>
const textActive = computed(() =>
  props.active ? "font-semibold" : "fontnormal"
);

const props = defineProps({
  active: {
    type: Boolean,
    default: false,
  },
});
</script>
