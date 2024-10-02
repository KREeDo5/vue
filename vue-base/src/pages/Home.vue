<script setup>
import Header from '../components/Header.vue'
import ProductList from '../components/ProductList.vue'

const items = [
  {
    id: 0,
    title: 'Микс Салатов, Соус Чили сладкий, Кинза',
    imageUrl: '/bull/salat-mix.png',
    weight: '300 г'
  },
  {
    id: 1,
    title: 'Стейк NY травяной',
    imageUrl: '/bull/steak-ny.png',
    weight: '250/70 г'
  },
  {
    id: 2,
    title: 'Стейк NY травяной',
    imageUrl: '/bull/steak-ny.png',
    weight: '250/70 г'
  },
  {
    id: 3,
    title: 'Стейк NY травяной',
    imageUrl: '/bull/steak-ny.png',
    weight: ''
  },
  {
    id: 4,
    title: 'Стейк NY травяной',
    imageUrl: '',
    weight: ''
  },
  {
    id: 5,
    title: '',
    imageUrl: '',
    weight: ''
  },
  {
    id: 6,
    title: '',
    imageUrl: '',
    weight: ''
  },
  {
    id: 7,
    title: '',
    imageUrl: '',
    weight: ''
  }
]
</script>

<template>
  <Header class="fixed top-0 left-0 right-0 z-10" />
  <!-- <Body /> -->
  <div class="bg-[url(/bull/the-bull.png)] min-h-screen bg-cover bg-no-repeat bg-fixed mt-20">
    <div class="bg-black/[.80] mx-20 py-6 px-20 rounded-3xl">
      <b class="text-[24px] text-white">Меню</b>
      <ProductList class="py-4" :items="items" />
    </div>
    <div class="bg-black/[.80] mx-20 mt-10 py-6 px-20 rounded-3xl">
      <b class="text-[24px] text-white">Наши рестораны</b>
    </div>
  </div>
  <!-- <Bottom /> -->
</template>
