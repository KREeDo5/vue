<script setup>
import { ref, computed } from 'vue'
import SafeNetworkImage from './SafeNetworkImage.vue'

const props = defineProps({
  title: String,
  weight: String,
  imageUrl: String,
  isFavorite: Boolean
})

const isFavorite = ref(false)

const onClick = () => {
  isFavorite.value = !isFavorite.value
}

const formattedWeight = computed(() => {
  return props.weight && props.weight.trim() ? `(${props.weight})` : null
})
</script>

<template>
  <div
    class="flex flex-col relative bg-[#303030]/80 rounded-3xl p-2 cursor-pointer hover:bg-[#303030]/90"
  >
    <img
      :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
      alt="favorite-icon"
      class="absolute top-6 right-6 z-0"
      @click="onClick"
    />
    <SafeNetworkImage :url="props.imageUrl" alt="product" class="rounded-2xl" />
    <p class="mt-2 text-white">{{ props.title || 'Без названия' }}</p>
    <p v-if="formattedWeight" class="text-[12px] text-[#C4C4C4]">{{ formattedWeight }}</p>
  </div>
</template>
