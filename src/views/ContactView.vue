<template>
  <section class="bg-white">
    <div class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12">
      <div class="max-w-md mr-auto place-self-center lg:col-span-7">
        <div>
          <div>
            <p class="flex text-lg py-5 font-bold">• HUBUNGI KAMI</p>
            <h1 class="">
              Kami bertanggung jawab memberikan kualitas produk yang terbaik untuk anda & keluarga,
              dan jika anda mengalami pengalaman yang buruk dengan produk kami anda dapat langsung
              menghubungi kami.
            </h1>
          </div>
          <div>
            <p class="flex text-lg py-5 font-bold">• HUBUNGI TOKO</p>
            <h1 class="">
              Untuk meningkatkan pelayanan pemesanan di sekitar anda, silahkan menghubungi outlet
              toko Hasil Karya kami yang berada disekitar anda. Pengiriman bebas biaya/gratis!
            </h1>
          </div>
        </div>
        <div class="w-full mt-5 grid grid-cols-2 gap-5 text-[#230F00]">
          <div>
            <p class="font-semibold">Kantor pusat</p>
            <div class="flex">
              <IconMail />
              <p>admin@hasilkarya.com</p>
            </div>
          </div>
          <div>
            <p class="font-semibold">Order</p>
            <div class="flex">
              <IconPhoneCall />
              <p>082183880808</p>
            </div>
          </div>
          <div>
            <p class="font-semibold">Customer Serivce</p>
            <div class="flex">
              <IconPhoneCall />
              <p>085256670000</p>
            </div>
          </div>
          <div>
            <p class="font-semibold">Kantor</p>
            <div class="flex">
              <IconPhoneCall />
              <p>(0431) 7283 995</p>
            </div>
          </div>
        </div>
      </div>
      <div class="w-auto flex-shrink-0 rounded-lg lg:mt-0 lg:col-span-5 lg:flex">
        <div class="card-body">
          <div class="form-control">
            <label class="label">
              <span class="label-text font-bold">Email</span>
            </label>
            <input type="text" placeholder="Email" class="input input-bordered" required />
          </div>
          <div class="form-control">
            <label class="label">
              <span class="label-text font-bold">Nomor Telpon</span>
            </label>
            <input type="number" placeholder="Nomor" class="input input-bordered" required />
          </div>
          <div class="form-control">
            <label class="label">
              <span class="label-text font-bold">Judul Pesan</span>
            </label>
            <input type="text" placeholder="Judul Pesan" class="input input-bordered" required />
          </div>
          <div class="form-control">
            <label class="label">
              <span class="label-text font-bold">Pesan</span>
            </label>
            <textarea
              placeholder="KETIK PESAN ANDA DISINI"
              class="textarea textarea-bordered textarea-lg w-full"
            ></textarea>
          </div>
          <div class="form-control mt-6">
            <button class="btn bg-[#230F00] text-white">KIRIM PESAN</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { IconPhoneCall, IconMail } from '@tabler/icons-vue'
</script>
