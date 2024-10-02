<script setup>
import Header from '../components/Header.vue'
import ProductList from '../components/ProductList.vue'
</script>

<template>
  <Header class="fixed top-0 left-0 right-0 z-10" />
  <!-- <Body /> -->
  <div class="bg-[url(/bull/the-bull.png)] min-h-screen bg-cover bg-no-repeat bg-fixed mt-20">
    <ProductList />
  </div>
  <!-- <Bottom /> -->
</template>
