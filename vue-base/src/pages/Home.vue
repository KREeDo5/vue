<script setup>
import Header from '../components/Header.vue'
import Card from '../components/Card.vue'
</script>

<template>
  <Header class="fixed top-0 left-0 right-0" />
  <!-- <Body /> -->
  <div class="bg-[url(/bull/the-bull.png)] min-h-screen bg-cover bg-no-repeat bg-fixed mt-20">
    <!-- Здесь билдим список -->
    <div class="grid grid-cols-4 gap-8 mx-60">
      <Card imageUrl="/bull/salat-mix.png" title="Микс Салатов, Соус Чили сладкий, Кинза (300 г)" />
      <Card imageUrl="/bull/steak-ny.png" title="Стейк NY травяной (250/70 г)" />
      <Card />
      <Card />
      <Card />
    </div>
  </div>
  <!-- <Bottom /> -->
</template>
