<script setup>
const props = defineProps({
  title: {
    type: String,
    default: "text",
  },
  description: {
    type: String,
    default: "text",
  },
  name: {
    type: String,
    default: "cart",
  },
});
</script>

<template>
  <div class="header-cart" v-if="name == 'cart'">
    <i class="fas fa-shopping-cart flex text-2xl lg:mr-2"></i>
    <span class="notification-cart">1</span>
    <span
      class="hidden lg:flex text-xs font-extrabold ml-1 text-center justify-center items-center"
      >Carrinho</span
    >
  </div>
  <div class="header-content-sm ml-1" v-else>
    <p class="leading-3">{{ title }}</p>
    <p class="font-extrabold">
      {{ description }}
      <i
        v-if="name != 'requests' && name != 'cart'"
        class="fas fa-chevron-down"
      ></i>
    </p>
  </div>
</template>

<style scoped></style>
