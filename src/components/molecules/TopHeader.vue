<script setup>
import HeaderContent from "../atoms/HeaderContent.vue";
</script>

<template>
  <div class="grid text-white">
    <div
      class="flex flex-wrap lg:flex-no-wrap bg-dark-blue-900 px-2 py-4 lg:py-1 items-center"
    >
      <div
        class="py-1 px-2 lg:border border-gray-700 hover:border-gray-400 rounded cursor-pointer"
      >
        <i class="fas fa-bars text-2xl"></i>
      </div>
      <div
        class="flex px-2 py-2 border border-transparent hover:border-gray-400 cursor-pointer"
      >
        <img src="../../assets/amazon_logo.png" alt="Amazon" class="h-7" /><span
          class="text-xs pl-1 pt-1"
          >.com.br</span
        >
      </div>
      <div
        class="w-full lg:w-auto flex-grow lg:ml-3 mr-0 pt-1 order-2 lg:order-none"
      >
        <form action="" class="flex">
          <select name="" id="" class="main-select">
            <option value="Livros">Livros</option>
          </select>
          <input type="text" class="p-2 flex-grow rounded-1 lg:rounded-none" />
          <button
            class="px-4 bg-gold-100 hover:bg-gold-200 rounded-tr rounded-br"
          >
            <i class="fas fa-search text-dark-blue-900 text-xl"></i>
          </button>
        </form>
      </div>
      <HeaderContent
        name="login"
        title="Olá, faça seu login"
        description="Contas e listas"
      />
      <HeaderContent
        name="request"
        title="Devoluções"
        description="e Pedidos"
      />
      <HeaderContent name="login" title="Experimente" description="Prime" />
      <HeaderContent name="cart" />
    </div>
  </div>
</template>

<style scoped></style>
