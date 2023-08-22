<template>
  <nav>
    <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-3">
      <a class="flex items-center">
        <img
          src="../assets/img/LOGO/logo_hasilkarya.png"
          class="h-[42.78px] w-[60px] md:h-[42.78px] md:w-[64px] lg:w-16 lg:h-10 mr-5"
          alt="Flowbite Logo"
        />
        <div class="grid w-12">
          <span class="self-center text-lg md:text-lg lg:text-2xl font-semibold whitespace-nowrap"
            >Hasil Karya</span
          >
        </div>
      </a>
      <button
        data-collapse-toggle="navbar-default"
        type="button"
        class="inline-flex items-center p-2 w-10 justify-center text-sm text-gray-500 rounded-lg lg:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
        aria-controls="navbar-default"
        aria-expanded="false"
        @click="toggleMenu"
      >
        <span class="sr-only">Open main menu</span>
        <IconAlignCenter />
      </button>
      <div
        :class="{ hidden: !openToggle }"
        class="w-full lg:block md:w-full lg:w-auto flex md:justify-center md:items-center bg-slate-400 bg-opacity-25 sm:bg-opacity-50 md:bg-opacity-20 lg:bg-transparent"
      >
        <ul
          class="font-medium flex flex-col px-11 mt-4 borderrounded-lg md:flex-row md:space-x-8 md:mt-0 md:border-0"
        >
          <li>
            <a>
              <RouterLink to="/" class="btn btn-ghost md:bg-transparent" aria-current="page">
                BERANDA
              </RouterLink>
            </a>
          </li>
          <li>
            <a>
              <RouterLink to="/about" class="btn btn-ghost" aria-current="page">
                <span class="">Tentang Kami</span>
              </RouterLink></a
            >
          </li>
          <li>
            <a>
              <RouterLink to="/about" class="btn btn-ghost" aria-current="page">
                <span class="">Produk</span>
              </RouterLink></a
            >
          </li>
          <li>
            <a>
              <RouterLink to="/about" class="btn btn-ghost" aria-current="page">
                <span class="">Kontak</span>
              </RouterLink></a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue'
import { IconAlignCenter } from '@tabler/icons-vue'
import { RouterLink } from 'vue-router'

const openToggle = ref(false)

const toggleMenu = () => {
  openToggle.value = !openToggle.value
}
</script>

<style scoped>
.font-brush {
  font-family: 'Brush Script MT', cursive;
}
</style>
