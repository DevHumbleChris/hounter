<script setup>
import Logo from "./Logo.vue";
</script>

<template>
  <header class="absolute top-0 right-0 left-0 p-5 z-40">
    <div class="flex items-center justify-between">
      <Logo />
      <div class="flex items-center justify-between space-x-16">
        <ul class="hidden md:flex items-center space-x-6">
          <li>
            <NuxtLink
              to="#"
              class="border bg-transparent text-semibold px-4 py-2 bg-[#96CBE5] text-white rounded-full"
              >About Us</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              to="#"
              class="border bg-transparent text-semibold px-4 py-2 bg-[#96CBE5] text-white rounded-full"
              >Article</NuxtLink
            >
          </li>
          <li>
            <select
              name="choice"
              class="bg-transparent outline-0 text-semibold border border-white px-4 py-2 bg-[#96CBE5] text-white rounded-full"
            >
              <option value="Property" selected>Property</option>
              <option value="Rented">Rented</option>
            </select>
          </li>
        </ul>
        <NuxtLink
          to="#"
          class="hidden md:block px-4 py-2 text-semibold bg-[#D1FAE5] text-[#047857] rounded-full"
          >Sign Up!</NuxtLink
        >
        <button aria-label="menu-hamburger" class="block md:hidden">
          <Icon name="charm:menu-hamburger" class="w-7 h-auto" />
        </button>
      </div>
    </div>
  </header>
</template>
