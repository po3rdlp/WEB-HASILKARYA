<template>
  <div class="bg-[#230F00] p-5">
    <footer class="p-5 text-white">
      <div class="flex justify-between">
        <div class="grid w-52">
          <img
            src="../assets/img/LOGO/logo_hasilkarya.png"
            class="w-[64px] h-[42.75]"
            alt="logo_hasilkarya"
          />
          <p class="mt-5">Lebih baik, beragam pilihan dan bernutrisi</p>
          <div class="flex gap-[24px] mt-5">
            <a href="https://www.facebook.com/hasilkaryamanado" target="_blank"
              ><IconBrandFacebookFilled
            /></a>
            <a
              href="https://grab.onelink.me/2695613898?pid=inappsharing&c=6-C3XWNJ5CL4KYUE&is_retargeting=true&af_dp=grab%3A%2F%2Fopen%3FscreenType%3DGRABMART%26sourceID%3DA4pcqCZkS4%26merchantIDs%3D6-C3XWNJ5CL4KYUE&af_force_deeplink=true&af_web_dp=https%3A%2F%2Fwww.grab.com%2Fdownload"
              target="_blank"
              ><IconCar
            /></a>
            <a href="https://www.instagram.com/hasilkarya/" target="_blank"
              ><IconBrandInstagram
            /></a>
          </div>
        </div>
        <div>
          <img
            src="../assets/img/LOGO/Logo_Perseroan_2.png"
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
import { IconCar, IconBrandFacebookFilled, IconBrandInstagram } from '@tabler/icons-vue'
</script>
