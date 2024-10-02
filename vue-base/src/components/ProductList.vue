<script setup>
import ProductCard from './ProductCard.vue'
</script>

<template>
  <div class="grid grid-cols-4 gap-8 mx-60">
    <ProductCard
      imageUrl="/bull/salat-mix.png"
      title="Микс Салатов, Соус Чили сладкий, Кинза (300 г)"
      :isFavorite="false"
    />
    <ProductCard
      imageUrl="/bull/steak-ny.png"
      title="Стейк NY травяной (250/70 г)"
      :isFavorite="true"
    />
    <ProductCard />
    <ProductCard />
    <ProductCard />
  </div>
</template>
