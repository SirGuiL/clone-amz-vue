<script setup>
import BottomNavItem from '../atoms/BottomNavItem.vue';

</script>

<template>
    <div class="flex text-black px-4 lg-2:px-0 text-xs border-b border-gray-300 bg-gray-100 pt-1">
        <a href="#" class="block lg-2:hidden py-2 font-bold">
            <i class="fas fa-chevron-left"></i> Todos os Departamentos
        </a>
        <ul class="hidden lg-2:flex">
            <BottomNavItem title="Livros" />
            <BottomNavItem title="Pesquisa avançada" />
            <BottomNavItem title="Mais vendidos" />
            <BottomNavItem title="Pré-venda e Lançamentos" />
            <BottomNavItem title="Livros em ofertas" />
            <BottomNavItem title="Inglês e outras línguas" />
            <BottomNavItem title="Loja Geek" />
            <BottomNavItem title="Universitários e Acadêmicos" />
            <BottomNavItem title="Didáticos e Escolares" />
            <BottomNavItem title="Loja Infantil" />
        </ul>
    </div>
</template>

<style scoped></style>
