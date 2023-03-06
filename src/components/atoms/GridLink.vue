<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
  isLast: {
    type: Boolean,
    default: false,
  },
});
</script>

<template>
  <li>
    <a
      href="#"
      :class="`text-blue-600 underline hover:text-orange-650 px-1 ${!isLast && 'border-r border-black'}`"
      >{{ title }}</a
    >
  </li>
</template>

<style scoped></style>
