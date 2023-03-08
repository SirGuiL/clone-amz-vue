<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
  image: {
    type: String,
    default: "text",
  },
  name: {
    type: String,
    default: "cart",
  },
  price: {
    type: Array,
  }
});
</script>

<template>
  <div class="w-1/2 lg:w-1/4 flex flex-col px-8 py-4 border-b border-r border-l border-gray-300">
    <img
      :src="`src/assets/${image}.jpg`"
      :alt="title"
      class="h-210px place-self-center p-2 cursor-pointer"
    />
    <p class="text-red-700 mt-10">R$ {{price[0]}}</p>
    <P class="text-sm mb-2"
      >De: <span class="line-through">R$ {{price[1]}}</span> ({{price[2]}} off)</P
    >
    <p class="text-xs text-gray-700 mb-2">Termina em 2:09:46</p>
    <a
      href="#"
      class="text-sm text-blue-600 hover:underline hover:text-orange-650 mb-2"
      >{{ title }}</a
    >
    <p class="text-sm mb-8">
      Esta oferta é exclusiva para membros do
      <a
        href="#"
        class="text-xs text-blue-600 hover:underline hover:text-orange-650"
      >
        Amazon Prime.
      </a>
    </p>
    <button class="text-xs bg-gray-200 border border-gray-600 rounded-sm py-1 mt-auto">
      Saiba Mais
    </button>
  </div>
</template>

<style scoped></style>
