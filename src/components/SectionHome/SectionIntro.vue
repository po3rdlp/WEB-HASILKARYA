<template>
  <section
    class="flex items-start lg:items-end min-h-screen md:min-h-max lg:h-[40rem] relative bg-[#F38630] z-10"
  >
    <div class="absolute bottom-0">
      <img
        src="../../assets/img/emojione-monotone_sheaf-of-rice_(1).png"
        class="max-w-full h-screen pointer-events-none opacity-100"
      />
    </div>
    <div class="flex w-full h-full">
      <div
        class="grid md:grid md:items-end lg:flex px-0 lg:px-5 py-10 ml-0 lg:ml-12 w-full z-50 relative"
      >
        <div class="">
          <div
            class="grid justify-end max-w-2xl md:max-w-md lg:max-w-2xl p-7 rounded-r-3xl text-[#230F00]"
          >
            <h1 class="text-2xl lg:text-5xl text-center lg:text-left font-bold">
              Lebih baik, beragam pilihan dan lebih bernutrisi
            </h1>
            <p class="py-6 text-center lg:text-left text-black w-full lg:w-96">
              Sebagai pabrik beras, kami berpengalaman, dan bekerjasama dengan para petani lokal
              yang berada di Nusantara.
            </p>
            <div class="flex justify-center lg:justify-start">
              <RouterLink to="/about">
                <button class="btn bg-[#230F00] hover:bg-black border-none text-white">
                  TENTANG KAMI
                </button></RouterLink
              >
            </div>
            <p class="py-6 text-center lg:text-left font-light text-xs w-full lg:w-96">
              "Sebagai pabrik beras, kami berpengalaman, dan bekerjasama dengan para petani lokal
              yang berada di Nusantara.""
            </p>
          </div>
        </div>
        <div>
          <div>
            <div class="flex justify-end items-end w-full">
              <img
                src="../../assets/img/Background.png"
                class="w-72 h-96 md:w-[22em] md:h-[16em] lg:w-[20em] lg:h-[27em] md:absolute md:bottom-0 lg:absolute lg:right-48 lg:bottom-0 pointer-events-none"
              />

              <img
                src="../../assets/img/sack-rice-with-rice-wooden-spoon-rice-plant_1.png"
                class="w-full h-96 md:w-[20em] md:h-[20em] lg:w-[27em] lg:h-[33em] absolute md:absolute lg:absolute bottom-0 right-0 pointer-events-none"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="absolute w-full -bottom-12 lg:bottom-0 z-50">
      <div class="flex justify-center w-full lg:h-auto lg:absolute lg:-bottom-11 lg:z-50">
        <div
          class="w-full p-3 lg:h-auto lg:w-fit lg:flex lg:justify-center items-center lg:space-x-10 rounded-lg"
        >
          <div
            class="grid grid-cols-5 w-full px-5 py-3 lg:h-auto lg:w-fit md:flex md:justify-center md:space-x-7 lg:flex lg:justify-center items-center lg:space-x-10 bg-white shadow-2xl rounded-lg"
          >
            <div class="w-24 h-12 lg:w-1/5 lg:h-auto lg:p-3">
              <img
                src="../../assets/img/LOGO/multimart.png"
                class="w-[81.84px] h-[21.83px] lg:w-[128px] lg:h-[34.13px] lg: mx-auto"
                alt="Multimart Logo"
              />
            </div>
            <div
              class="md:border-r md:border-gray-300 md:h-12 lg:border-r lg:border-gray-300 lg:h-12"
            ></div>

            <div class="w-24 h-8 lg:w-1/5 lg:h-auto lg:p-3">
              <img
                src="../../assets/img/LOGO/alfamart.png"
                class="w-[81.84px] h-[20.13px] lg:w-[128px] lg:h-[34.13px] mx-auto"
                alt="Alfamart Logo"
              />
            </div>
            <div
              class="md:border-r md:border-gray-300 md:h-12 lg:border-r lg:border-gray-300 lg:h-12"
            ></div>

            <div class="w-20 h-10 lg:w-1/5 lg:h-auto lg:p-3">
              <img
                src="../../assets/img/LOGO/indomart.png"
                class="w-[81.84px] h-[26.6] lg:w-[128px] lg:h-[34.13px] mx-auto"
                alt="Indomart Logo"
              />
            </div>
            <div
              class="md:border-r md:border-gray-300 md:h-12 lg:border-r lg:border-gray-300 lg:h-12"
            ></div>

            <div class="w-24 h-11 lg:w-1/5 lg:h-auto lg:p-3">
              <img
                src="../../assets/img/LOGO/indgrosir.png"
                class="w-[81.84px] h-[28.61px] lg:w-[128px] lg:h-[34.13px] mx-auto"
                alt="Indogrosir Logo"
              />
            </div>
            <div
              class="md:border-r md:border-gray-300 md:h-12 lg:border-r lg:border-gray-300 lg:h-12"
            ></div>

            <div class="w-24 h-10 lg:w-1/5 lg:h-auto lg:p-3">
              <img
                src="../../assets/img/LOGO/transmart.png"
                class="w-[81.84px] h-[10.71px] lg:w-[128px] lg:h-[16.75px] mx-auto"
                alt="Transmart Logo"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
