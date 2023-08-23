<template>
  <div class="w-full h-full p-5">
    <div class="grid sm:flex justify-around items-center">
      <div class="max-w-sm lg:max-w-3xl">
        <div class="max-w-lg">
          <h1 class="flex text-lg py-5 font-bold">• TEMUKAN KAMI</h1>
          <h1 class="flex text-3xl font-bold">PT. Hasil Karya Sentra Pangan</h1>
          <p class="py-6">
            Jaga III, Desa/Kelurahan Kalasey satu, Kec. Mandolang, Kab. Minahasa, Provinsi Sulawesi
            Utara, 95661
          </p>

          <RouterLink to="/about" class="btn bg-[#230F00] text-white"
            >BUKA DI GOOGLE MAPS</RouterLink
          >
        </div>
      </div>
      <div class="flex justify-center items-center p-1 mt-5 md:p-3 lg:p-5 xl:p-7 2xl:p-10">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1477.8322456493543!2d124.77353622867471!3d1.4585746605849186!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x328775087f5ff57b%3A0x1e0cbea08352a24e!2sPT%20Hasil%20Karya%20Sentra%20Pangan!5e0!3m2!1sid!2sid!4v1692676151425!5m2!1sid!2sid"
          class="w-full h-96 md:w-80 lg:w-96 rounded-lg"
          style="border: 0"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </div>
  </div>
</template>
