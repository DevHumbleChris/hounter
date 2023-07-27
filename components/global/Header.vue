<script setup>
import Logo from "./Logo.vue";
import { Dialog, DialogPanel } from "@headlessui/vue";
import { XMarkIcon } from "@heroicons/vue/24/outline";

const mobileMenuOpen = useState("mobileMenuOpen", () => false);
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
              name="choice" aria-label="choice-selection"
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
        <button
          @click="mobileMenuOpen = true"
          aria-label="menu-hamburger"
          class="block md:hidden"
        >
          <Icon name="charm:menu-hamburger" class="w-7 h-auto" />
        </button>

        <!-- Mobile Menu -->
        <Dialog
          as="div"
          class="lg:hidden"
          @close="mobileMenuOpen = false"
          :open="mobileMenuOpen"
        >
          <div class="fixed inset-0 z-50" />
          <DialogPanel
            class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
          >
            <div class="flex items-center justify-between">
              <a href="#" class="-m-1.5 p-1.5">
                <span class="sr-only">Jadoo</span>
                <Logo />
              </a>
              <button
                type="button"
                class="-m-2.5 rounded-md p-2.5 text-gray-700"
                @click="mobileMenuOpen = false"
                aria-label="close"
              >
                <span class="sr-only">Close menu</span>
                <XMarkIcon class="h-6 w-6" aria-hidden="true" />
              </button>
            </div>
            <div class="mt-6 flow-root">
              <div class="-my-6 divide-y divide-gray-500/10">
                <div class="space-y-2 py-6">
                  <NuxtLink
                    to="#"
                    class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                    >About Us</NuxtLink
                  >
                  <NuxtLink
                    to="#"
                    class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                    >Article</NuxtLink
                  >
                  <select
              name="choice" aria-label="choice-selection"
              class="-mx-2 block rounded-lg px-1 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50 outline-0"
            >
              <option value="Property" selected>Property</option>
              <option value="Rented">Rented</option>
            </select>
                </div>
                <div class="py-6 space-y-4">
                  <NuxtLink
                    to="#"
                    class="-mx-3 block rounded-lg px-3 py-2.5 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50"
                    >Signup</NuxtLink
                  >
                </div>
              </div>
            </div>
          </DialogPanel>
        </Dialog>
      </div>
    </div>
  </header>
</template>
