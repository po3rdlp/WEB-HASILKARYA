<template>
  <div class="hero min-h-screen xl:h-full 2xl:h-full bg-base-200 z-10 mt-5 md:mt-5 lg:mt-0">
    <div class="hero-content flex-col-reverse lg:flex-row-reverse">
      <div class="relative p-5 lg:p-10">
        <img
          src="../../assets/img/image.png"
          class="w-96 md:max-w-md lg:max-w-lg rounded-lg transition ease-in-out delay-150 hover:scale-110 hover:bg-none duration-300 text-neutral-content"
        />
      </div>
      <div class="max-w-lg">
        <h1 class="flex text-lg py-5 font-bold">• Latar Belakang</h1>
        <h1 class="flex text-3xl font-bold">
          <InfoCircleIcon class="mr-2" />Dipercaya Selama 43 Tahun
        </h1>
        <p class="py-6">
          Sejak tahun 1971, kami beroperasi sebagai pelopor dalam pengolahan bahan pokok beras di
          Indonesia. Dimulai dengan Toko Karya Jaya, nama kami semakin dikenal seiring waktu. Pada
          1984, UD. Hasil Karya didirikan dan memperkenalkan teknologi Rice Polishing. Transformasi
          berlanjut, dan pada tahun 2017, lahirlah PT. Hasil Karya Sentra Pangan. Kami berkomitmen
          memberikan produk beras terbaik, higienis, dan berkualitas premium bagi masyarakat
          Indonesia.
        </p>

        <RouterLink to="/about" class="btn btn-ghost text-[#FA6900]">SELENGKAPNYA</RouterLink>
      </div>
    </div>
  </div>
</template>

<script setup></script>
