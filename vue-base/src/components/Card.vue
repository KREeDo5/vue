<script setup>
import { ref } from 'vue'
import SafeNetworkImage from '../components/SafeNetworkImage.vue'

defineProps({
  title: String,
  imageUrl: String,
})

const isLiked = ref(false)

const onClick = () => {
  isLiked.value = !isLiked.value
}
</script>

<template>
  <div
    class="flex flex-col relative bg-white border-slate-100 rounded-3xl p-2 cursor-pointer hover:bg-relative-200"
  >
    <img src="/like-2.svg" alt="favorite-icon" class="absolute top-6 right-6" />
    <SafeNetworkImage :url="imageUrl" alt="product" class="rounded-2xl" />
    <p class="mt-2">{{ title }}</p>
  </div>
</template>
