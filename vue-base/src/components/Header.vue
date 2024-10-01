<template>
  <header class="flex justify-between bg-black px-8 py-2">
    <div class="flex flex-col items-center cursor-pointer text-white">
      <img src="/logo.svg" alt="Logo" class="w-40" />
      <p>мясной ресторан</p>
    </div>

    <ul class="flex items-center gap-8">
      <li class="flex gap-2 cursor-pointer">
        <img src="/bull/vk.png" alt="vk" class="h-6 object-cover" />
      </li>
      <li class="flex gap-2 cursor-pointer">
        <img src="/bull/telegram.png" alt="tg" class="h-6 object-cover" />
      </li>
      <li class="flex gap-2 cursor-pointer text-white hover:text-slate-300">
        <img src="/cart.svg" alt="Cart" class="h-6 object-cover" />
        <span>999 руб.</span>
      </li>
      <li class="flex gap-2 cursor-pointer text-white hover:text-slate-300">
        <img src="/heart.svg" alt="Favorite" class="h-6 object-cover" />
        <span>Избранное</span>
      </li>
      <li class="flex gap-2 cursor-pointer text-white hover:text-slate-300">
        <img src="/profile.svg" alt="Profile" class="h-6 object-cover" />
        <span>Профиль</span>
      </li>
    </ul>
  </header>
</template>
