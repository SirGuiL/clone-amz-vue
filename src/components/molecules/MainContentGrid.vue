<script setup>
import GridLink from '../atoms/GridLink.vue';
import Banner from '../atoms/Banner.vue';
import RoundedCard from '../atoms/RoundedCard.vue';
import ProductCard from '../atoms/ProductCard.vue';
</script>

<template>
  <div class="col-span-6 lg:col-span-5 p-2">
    <div class="flex flex-col">
        <div class="text-center">
            <h2 class="text-2xl font-bold lg:text-3xl lg:font-normal">Loja de Livros</h2>
            <ul class="flex flex-wrap lg:flex-now-wrap justify-center lg:text-sm px-4 lg:px-0 pb-2 mt-3">
                <GridLink title="Livros em Oferta" />
                <GridLink title="Importados" />
                <GridLink title="Lançamentos" />
                <GridLink title="Universitários" />
                <GridLink title="Didáticos e Escolares" />
                <GridLink title="HQs e Mangás" />
                <GridLink title="Mais Vendidos" />
                <GridLink title="Livros Infantis" />
                <GridLink title="Indicações" isLast />
            </ul>
            <div class="h-2 border-b shadow-md"></div>
        </div>
        <Banner />
        <div class="flex flex-col lg:flex-row items-center my-8 py-1">
          <p class="font-bold lg:w-3/4 text-center lg:border-r-2 border-gray-300 leading-5 pr-2 mt-10 lg:mt-0">
            Assine o Amazon Prime para ter benefícios de leitura com o Prime Reading, frete GRÁTIS sem valor mínimo de compra e muito mais. Apenas R$ 9,90/mês
          </p>
          <a href="#" class="free-trial-btn">Teste GRÁTIS por 30 dias</a>
        </div>
        <div class="flex flex-col px-6 pb-8 border-b border-gray-300">
          <h3 class="text-center lg:text-left text-xl font-bold mb-4">
            Encontre ofertas por categorias
          </h3>
          <ul class="flex flex-wrap justify-center lg:justify-start lg:flex-no-wrap px-2 text-xs font-bold">
            <RoundedCard title="Todas as Ofertas"  />
            <RoundedCard title="Ofertas Relâmpago" :index="2"  />
            <RoundedCard title="Literatura" :index="3" />
            <RoundedCard title="HQs e Mangás" :index="4" />
            <RoundedCard title="Ficção" :index="5" />
            <RoundedCard title="Inglês e Outras Línguas" :index="6" />
            <RoundedCard title="Autoajuda" :index="7" />
            <RoundedCard title="Infantil" :index="8" />
            <RoundedCard title="Negócios" :index="9" />
          </ul>
        </div>
        <div class="flex flex-col">
          <div class="flex justify-between py-2 px-4 text-sm">
            <p>Mostrando 1-32 de 122 Resultados</p>
            <div class="flex lg:flex-none">
              <span>Ordenar por</span>
              <select name="" id="" class="bg-gray-300 pr-4 lg:pr-12 ml-3 rounded-sm border border-gray-600 text-xs px-1">
                <option value="Destaques">Destaques</option>
              </select>
            </div>
          </div>
          <div class="flex flex-wrap border-gray-300 divide-gray-300 mb-10 mt-10">
            <ProductCard title="Em busca de sentido" image="livro1" :price="['26,30', '63,60', '58%']" />
            <ProductCard title="Não se humilha, não" image="livro2" :price="['17,40', '39,90', '56%']" />
            <ProductCard title="As seis lições" image="livro3" :price="['17,40', '34,90', '50%']" />
            <ProductCard title="Anne II" image="livro4" :price="['27,90', '49,90', '44%']" />
            <ProductCard title="Propósito - A Coragem de ser quem somos" image="livro5" :price="['13,40', '39,90', '66%']" />
            <ProductCard title="A morte de Ivan Ilitch" image="livro6" :price="['20,50', '42,00', '51%']" />
            <ProductCard title="Outros jeitos de usar a boca" image="livro7" :price="['10,40', '37,90', '73%']" />
            <ProductCard title="Nassim Nicholas Taleb - Kit exclusivo Amazon" image="livro8" :price="['55,90', '119,90', '53%']" />
          </div>
        </div>
    </div>
  </div>
</template>

<style scoped></style>
