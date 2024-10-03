<script setup>
import Header from './components/Header.vue'
</script>

<template>
  <Header class="header fixed top-0 left-0 right-0 z-10" />
  <main>
    <div class="flex justify-center text-white bg-red-500">03.09-03.10 Скидка 20% на все блюда</div>
    <RouterView />
  </main>
</template>
