<template>
  <div class="w-full h-full p-1 lg:px-5 lg:py-5 lg:p-3 bg-[#F38630]">
    <div class="flex justify-between p-5">
      <div>
        <h1 class="flex text-lg py-5 font-bold">• PRODUK TERBAIK KAMI</h1>
      </div>
      <div class="flex items-center gap-5">
        <IconCircleArrowLeftFilled />
        <IconCircleArrowRightFilled />
      </div>
    </div>

    <div class="flex gap-2 lg:gap-5 overflow-x-auto">
      <div class="card w-full h-full bg-base-100 rounded-3xl relative">
        <div class="flex justify-end p-2">
          <IconHeartFilled class="z-10 text-red-500" />
        </div>
        <figure>
          <img
            src="../../assets/img/Products/Products.png"
            class="w-full absolute top-0 h-full"
            alt="Shoes"
          />
          <img src="../../assets/img/Products/Dua_Merpati_5kg.png" class="max-w-xs" alt="Shoes" />
        </figure>
        <div class="p-3 z-10">
          <div class="flex justify-between">
            <p class="text-white">BERAS DUA MERPATI 5KG</p>
            <a aria-label="Chat on WhatsApp" href="https://wa.me/99999910" target="_blank">
              <button class="btn btn-primary">Pesan</button>
            </a>
          </div>
        </div>
      </div>
      <div class="card w-full h-full bg-base-100 rounded-3xl relative">
        <div class="flex justify-end p-2">
          <IconHeartFilled class="z-10 text-red-500" />
        </div>
        <figure>
          <img
            src="../../assets/img/Products/Products.png"
            class="w-full absolute top-0 h-full"
            alt="Shoes"
          />
          <img src="../../assets/img/Products/Dua_Merpati_10kg.png" class="max-w-xs" alt="Shoes" />
        </figure>
        <div class="p-3 z-10">
          <div class="flex justify-between">
            <p class="text-white">BERAS DUA MERPATI 10KG</p>
            <a aria-label="Chat on WhatsApp" href="https://wa.me/99999910" target="_blank">
              <button class="btn btn-primary">Pesan</button>
            </a>
          </div>
        </div>
      </div>
      <div class="card w-full h-full bg-base-100 rounded-3xl relative">
        <div class="flex justify-end p-2">
          <IconHeartFilled class="z-10 text-red-500" />
        </div>
        <figure>
          <img
            src="../../assets/img/Products/Products.png"
            class="w-full absolute top-0 h-full"
            alt="Shoes"
          />
          <img src="../../assets/img/Products/Dua_Merpati_20kg.png" class="max-w-xs" alt="Shoes" />
        </figure>
        <div class="p-3 z-10">
          <div class="flex justify-between">
            <p class="text-white">BERAS DUA MERPATI 20KG</p>
            <a aria-label="Chat on WhatsApp" href="https://wa.me/99999910" target="_blank">
              <button class="btn btn-primary">Pesan</button>
            </a>
          </div>
        </div>
      </div>
      <div class="card w-full h-full bg-base-100 rounded-3xl relative">
        <div class="flex justify-end p-2">
          <IconHeartFilled class="z-10 text-red-500" />
        </div>
        <figure>
          <img
            src="../../assets/img/Products/Products.png"
            class="w-full absolute top-0 h-full"
            alt="Shoes"
          />
          <img src="../../assets/img/Products/Istana_Pangan_5kg.png" class="max-w-xs" alt="Shoes" />
        </figure>
        <div class="p-3 z-10">
          <div class="flex justify-between">
            <p class="text-white">ISTANA PANGAN 5KG</p>
            <a aria-label="Chat on WhatsApp" href="https://wa.me/99999910" target="_blank">
              <button class="btn btn-primary">Pesan</button>
            </a>
          </div>
        </div>
      </div>
      <div class="card w-full h-full bg-base-100 rounded-3xl relative">
        <div class="flex justify-end p-2">
          <IconHeartFilled class="z-10 text-red-500" />
        </div>
        <figure>
          <img
            src="../../assets/img/Products/Products.png"
            class="w-full absolute top-0 h-full"
            alt="Shoes"
          />
          <img
            src="../../assets/img/Products/Istana_Pangan_10kg.png"
            class="max-w-xs"
            alt="Shoes"
          />
        </figure>
        <div class="p-3 z-10">
          <div class="flex justify-between">
            <p class="text-white">ISTANA PANGAN 10KG</p>
            <a aria-label="Chat on WhatsApp" href="https://wa.me/99999910" target="_blank">
              <button class="btn btn-primary">Pesan</button>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import {
  IconHeartFilled,
  IconCircleArrowLeftFilled,
  IconCircleArrowRightFilled
} from '@tabler/icons-vue'
</script>
