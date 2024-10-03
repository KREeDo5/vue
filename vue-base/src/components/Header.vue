<template>
  <header class="header-padding flex justify-between bg-black">
    <RouterLink to="/">
      <div class="flex flex-col items-center cursor-pointer text-white">
        <img src="/logo.svg" alt="Logo" class="w-40" />
        <p>мясной ресторан</p>
      </div>
    </RouterLink>
    <ul class="flex items-center gap-8">
      <li class="flex gap-2 cursor-pointer">
        <a href="https://vk.com/thebullmsk" target="_blank">
          <img src="/bull/vk.png" alt="vk" class="h-6 object-cover" />
        </a>
      </li>
      <li class="flex gap-2 cursor-pointer">
        <a href="https://t.me/bullmyaso" target="_blank">
          <img src="/bull/telegram.png" alt="tg" class="h-6 object-cover" />
        </a>
      </li>
      <li class="flex gap-2 cursor-pointer text-white hover:text-[#C4C4C4]">
        <img src="/cart.svg" alt="Cart" class="h-6 object-cover" />
        <span>999 руб.</span>
      </li>
      <RouterLink to="/favorite">
        <li class="flex gap-2 cursor-pointer text-white hover:text-[#C4C4C4]">
          <img src="/heart.svg" alt="Favorite" class="h-6 object-cover" />
          <span>Избранное</span>
        </li>
      </RouterLink>
      <RouterLink to="/profile">
        <li class="flex gap-2 cursor-pointer text-white hover:text-[#C4C4C4]">
          <img src="/profile.svg" alt="Profile" class="h-6 object-cover" />
          <span>Профиль</span>
        </li>
      </RouterLink>
    </ul>
  </header>
</template>

<style scoped>
.header-padding {
  padding: 8px 16px;
}
</style>
