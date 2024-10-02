<script setup>
import { ref } from 'vue'
import SafeNetworkImage from './SafeNetworkImage.vue'

defineProps({
  title: String,
  imageUrl: String,
  isFavorite: Boolean
})

const isFavorite = ref(false)

const onClick = () => {
  isFavorite.value = !isFavorite.value
}
</script>

<template>
  <div
    class="flex flex-col relative bg-white border-slate-100 rounded-3xl p-2 cursor-pointer hover:bg-relative-200"
  >
    <img
      :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
      alt="favorite-icon"
      class="absolute top-6 right-6 z-0"
      @click="onClick"
    />
    <SafeNetworkImage :url="imageUrl" alt="product" class="rounded-2xl" />
    <p class="mt-2">{{ title }}</p>
  </div>
</template>
