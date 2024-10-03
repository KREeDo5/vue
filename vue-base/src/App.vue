<script setup>
import Header from './components/Header.vue'
</script>

<template>
  <Header class="fixed top-0 left-0 right-0 z-10" />
  <main class="mt-20">
    <nav>
      <RouterLink to="/">Go to Home</RouterLink>
      <RouterLink to="/favorite">Go to Favorite</RouterLink>
    </nav>
    <RouterView />
  </main>
</template>
