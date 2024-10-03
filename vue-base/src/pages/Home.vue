<script setup>
import { onMounted, ref } from 'vue'
import axios from 'axios'

import ProductList from '../components/ProductList.vue'

const items = ref([])

onMounted(async () => {
  // fetch('https://58eb93e5f4cd62bd.mokky.dev/menu')
  //   .then((response) => response.json())
  //   .then((data) => {
  //     console.log(data)
  //   })

  try {
    const { data } = await axios.get('https://58eb93e5f4cd62bd.mokky.dev/menu')
    items.value = data
  } catch (e) {
    console.log(e)
  }
})
</script>

<template>
  <div class="bg-[url(/bull/the-bull.png)] min-h-screen bg-cover bg-no-repeat bg-fixed">
    <div class="delivery-card text-white text-[14px]">
      <div class="icon-text gap-2">
        <img src="/bull/clock.svg" alt="Clock" class="h-4 object-cover" />
        <p class="text-[16px]">Время приема заказов</p>
      </div>
      <p>– на доставку с 12:00 до 22:00</p>
      <p>– на самовывоз с 12:00 до 23:00</p>
    </div>
    <div class="bg-black/[.80] mx-20 py-6 px-20 rounded-3xl">
      <b class="text-[24px] text-white">Меню</b>
      <ProductList class="py-4" :items="items" />
    </div>
    <div class="bg-black/[.80] mx-20 mt-10 py-6 px-20 rounded-3xl">
      <b class="text-[24px] text-white">Наши рестораны</b>
    </div>
  </div>
</template>

<style scoped>
.delivery-card {
  background: linear-gradient(90deg, rgba(213, 31, 48, 0.7) 0%, rgba(161, 21, 34, 0.51) 100%);
  padding: 12px 20px;
  border-radius: 24px;
  width: max-content; /* Минимальная необходимая ширина */
  align-items: center;
  margin: 10px 80px;
}
.icon-text {
  display: inline-flex;
  align-items: center;
}
</style>
