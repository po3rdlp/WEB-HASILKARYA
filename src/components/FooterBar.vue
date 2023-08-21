<template>
  <div class="bg-[#230F00] p-5">
    <footer class="p-5 text-white">
      <div class="flex justify-between">
        <div class="grid w-52">
          <img
            src="../assets/img/LOGO/logo_hasilkarya.png"
            class="w-20 h-14"
            alt="logo_hasilkarya"
          />
          <p class="mt-5">Lebih baik, beragam pilihan dan bernutrisi</p>
          <div class="flex gap-[24px] mt-5">
            <IconBrandFacebookFilled />
            <IconBrandTwitterFilled />
            <IconBrandInstagram />
          </div>
        </div>
        <div>
          <img
            src="../assets/img/LOGO/Logo Perseroan 2.png"
            class="w-20 h-20"
            alt="logo_perseroan"
          />
        </div>
      </div>
    </footer>
    <footer class="footer p-5 border-t text-white border-base-300">
      <div class="items-center grid-flow-col">
        <p>©2022 Company Name. All rights reserved</p>
      </div>
      <div class="md:place-self-center md:justify-self-end">
        <div class="flex justify-evenly gap-4">
          <p>KEBIJAKAN PRIVASI</p>
          <p>Syarat & Ketentuan</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import {
  IconBrandTwitterFilled,
  IconBrandFacebookFilled,
  IconBrandInstagram
} from '@tabler/icons-vue'
</script>
