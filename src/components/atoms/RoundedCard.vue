<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
  index: {
    type: Number,
    default: 1,
  },
});
</script>

<template>
  <li class="text-center mx-3 mb-4 lg:mb-0">
    <img
      :src="`src/assets/cat${index}.jpg`"
      :alt="title"
      class="rounded w-full lg:w-75px mb-2 mx-auto cursor-pointer"
    />
    <a href="#" class="lg:flex lg:text-center lg:justify-center lg:w-24">{{title}}</a>
  </li>
</template>

<style scoped></style>
