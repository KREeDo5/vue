<script setup>
import { ref } from 'vue'

let count = ref(0)

function increment() {
  count.value++
  console.log(count)
}
</script>

<template>
  <h1>{{ count }}</h1>
  <button @click="increment">+</button>
</template>
