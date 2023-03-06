<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
});
</script>

<template>
  <li class="bottom-nav-link">{{title}}</li>
</template>

<style scoped></style>
