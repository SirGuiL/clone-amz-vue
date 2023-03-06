<script setup>
import LeftList from "../atoms/LeftList.vue";
</script>

<template>
  <div
    class="col-span-1 h-screen hidden lg:block pl-2 my-2 border-r border-gray-300 text-xs"
  >
    <LeftList
      title="Destaque em Livros"
      :links="[
        'Indicações Amazon',
        'Inglês e Outras Línguas',
        'Livros em Oferta',
        'Mais Vendidos do Mês',
        'Pré-venda e Lançamentos',
        'Livros Exclusivos Amazon',
      ]"
    />
    <LeftList
      title="Páginas Especiais"
      :links="[
        'Livros Clássicos',
        'Livros Que Viraram Filmes',
        'Livros Infantis',
        'Loja Geek'
      ]"
    />
    <LeftList
      title="Livros Educacionais"
      :links="[
        'Didáticos e Escolares',
        'Estudo e Ensino de Idiomas',
        'Exames e Concursos',
        'Importados para Exames',
        'Universitários e Acadêmicos',
        'Livros Exclusivos Amazon',
      ]"
    />
    <LeftList
      title="Kindle"
      :links="[
        'Acessórios Kindle',
        'Comprar Kindle',
        'e-Books em Inglês',
        'e-Books em Oferta',
        'Kindle Unlimited',
        'Todos os e-Books',
      ]"
    />
  </div>
</template>

<style scoped></style>
