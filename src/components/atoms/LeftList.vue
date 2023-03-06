<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
  links: {
    type: Array,
    required: true
  }
});
</script>

<template>
  <h3 class="font-bold">{{ title }}</h3>
    <ul class="pl-2 mb-2">
        <li class="text-gray-800 hover:text-orange-650" v-for="link in links">
            <a href="#">{{link}}</a>
        </li>
    </ul>
</template>

<style scoped></style>
