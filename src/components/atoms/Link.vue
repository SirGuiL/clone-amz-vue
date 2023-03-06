<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
});
</script>

<template>
  <li
    class="link"
  >
    <a href="#">{{ title }}</a>
  </li>
</template>

<style scoped></style>
