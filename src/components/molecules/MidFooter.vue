<script setup>
import CountryLink from "../atoms/CountryLink.vue";
</script>

<template>
  <div
    class="hidden lg:flex flex-col items-center bg-dark-blue-700 border-t border-gray-700 pt-6 pb-4"
  >
    <img src="src/assets/amazon_logo.png" alt="Amazon" class="w-20" />
    <ul class="flex flex-wrap justify-center text-xs pt-4 text-gray-400 w-3/4">
      <CountryLink title="Austrália" />
      <CountryLink title="Alemanha" />
      <CountryLink title="Canadá" />
      <CountryLink title="China" />
      <CountryLink title="Cingapura" />
      <CountryLink title="Espanha" />
      <CountryLink title="Estados Unidos" />
      <CountryLink title="França" />
      <CountryLink title="Holanda" />
      <CountryLink title="Índia" />
      <CountryLink title="Itália" />
      <CountryLink title="Japão" />
      <CountryLink title="México" />
      <CountryLink title="Emirados Árabes Unidos" />
      <CountryLink title="Reino Unido" />
      <CountryLink title="Turquia" isLast />
    </ul>
  </div>
</template>

<style scoped></style>
