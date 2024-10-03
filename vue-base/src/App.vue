<script setup>
import Header from './components/Header.vue'
</script>

<template>
  <header>
    <Header class="header fixed top-0 left-0 right-0 z-10" />
  </header>
  <main>
    <RouterView />
  </main>
</template>
