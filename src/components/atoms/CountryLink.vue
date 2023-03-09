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
  <li :class="`px-2 ${!isLast && 'border-r border-gray-600'} hover:underline`">
    <a href="#">{{title}}</a>
  </li>
</template>

<style scoped></style>
