<script setup>
defineProps({
  url: String
})
</script>

<template>
  <img :src="url || '/bull/placeholder.png'" alt="network-image" />
</template>
