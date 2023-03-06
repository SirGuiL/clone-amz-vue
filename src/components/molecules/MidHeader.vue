<script setup>
import Link from "../atoms/Link.vue";
</script>

<template>
  <div class="flex bg-dark-blue-600 text-sm px-2 py-1 items-center text-white">
    <div
      class="flex items-center border border-transparent hover:border-gray-400 rounded-sm px-2 py-2 lg:py-0 cursor-pointer"
    >
      <div class="mr-1 lg:mr-3">
        <i class="fas fa-map-marker-alt text-xl"></i>
      </div>
      <div class="flex lg:block leading-tight text-xs">
        <p class="mx-1 lg:mx-0">Olá</p>
        <p class="font-bold">Selecione o endereço</p>
      </div>
    </div>
    <div class="hidden lg:block">
      <nav>
        <ul class="flex ml-10 text-sm">
          <Link title="Mais vendidos" />
          <Link title="Livros" />
          <Link title="Ofertas do dia" />
          <Link title="Atendimento ao cliente" />
          <Link title="Eletrônicos" />
          <Link title="Ideias para presente" />
        </ul>
      </nav>
    </div>
  </div>
</template>

<style scoped></style>
