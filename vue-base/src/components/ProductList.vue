<script setup>
import ProductCard from './ProductCard.vue'

defineProps({
  items: Array
})
</script>

<template>
  <div class="grid grid-cols-4 gap-8">
    <ProductCard
      v-for="item in items"
      :key="item.id"
      :imageUrl="item.imageUrl"
      :title="item.title"
      :weight="item.weight"
    />
  </div>
</template>
