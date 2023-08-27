<template>
  <dialog
    :open="showMQ"
    v-if="Produk"
    class="modal modal-bottom sm:modal-middle bg-gray-500 bg-opacity-80"
  >
    <div class="modal-box">
      <div class="flex justify-between gap-5">
        <div class="border border-gray-400 shadow-xl rounded-lg p-3">
          <p class="text text-sm text-center">{{ Produk.NamaProduk }}</p>
          <img :src="Produk.image" alt="image" class="w-56 h-56" />
          <p class="flex text-xs text-center pb-5 font-bold">Rp {{ Produk.Harga }}</p>
          <div class="flex items-center gap-1">
            <button
              type="button"
              class="w-10 h-10 leading-10 text-white transition hover:opacity-75 bg-gray-500 rounded-lg"
              @click="minusButton"
            >
              &minus;
            </button>
            <input
              type="number"
              v-model="quantity"
              v-on:change="quantity"
              class="h-10 w-16 rounded border-gray-200 text-center [-moz-appearance:_textfield] sm:text-sm [&::-webkit-outer-spin-button]:m-0 [&::-webkit-outer-spin-button]:appearance-none [&::-webkit-inner-spin-button]:m-0 [&::-webkit-inner-spin-button]:appearance-none"
            />
            <button
              type="button"
              @click="plusButton"
              class="w-10 h-10 leading-10 text-white transition hover:opacity-75 bg-gray-500 rounded-lg"
            >
              &plus;
            </button>
          </div>
          <label class="label cursor-pointer gap-2">
            <span class="label-text text-xs font-bold text-black">Delivery</span>
            <input
              type="checkbox"
              class="checkbox checkbox-primary"
              @change="toggleDelivery"
              :checked="selectedCategory === 'Delivery'"
              required
            />
            <span class="label-text text-xs font-bold text-black">Pick Up</span>
            <input
              type="checkbox"
              class="checkbox checkbox-primary"
              @change="togglePickup"
              :checked="selectedCategory === 'Pick Up'"
              required
            />
          </label>
          <div v-if="selectedCategory === 'Delivery'">
            <label class="label text-sm">Alamat Pengiriman:</label>
            <input
              class="input input-sm w-full"
              placeholder="Alamat Pengiriman"
              v-model="deliveryAddress"
              required
            />
            <p class="text-xs font-light pt-5">"MOHON MASUKAN ALAMAT DENGAN JELAS"</p>
          </div>
        </div>
        <div class="w-full border border-gray-400 shadow-xl rounded-lg p-3">
          <label class="label">Masukan Nama: </label>
          <input class="input" placeholder="Nama" v-model="personName" required />
          <label class="label">Nama Perusahaan/Pembeli</label>
          <input class="input" placeholder="Company Name" v-model="companyName" required />
          <div class="form-control">
            <label class="label">
              <span class="label-text">Deskripsi</span>
            </label>
            <textarea
              placeholder="Deskripsi Pemesanan"
              class="textarea text-sm textarea-bordered textarea-lg w-full"
              v-model="desc"
              required
            ></textarea>
          </div>
        </div>
      </div>
      <div class="modal-action">
        <a aria-label="Chat on WhatsApp" :href="whatsappLink" target="_blank">
          <p class="btn btn-primary">Pesan</p>
        </a>
        <button class="btn btn-warning" @click="closeModal">Close</button>
      </div>
    </div>
  </dialog>
</template>

<script>
export default {
  props: {
    showMQ: Boolean,
    Produk: {
      type: Object,
      required: true
    }
  },
  data() {
    return {
      quantity: 1,
      totalHarga: 0,
      personName: '',
      companyName: '',
      desc: '',
      deliveryAddress: '',
      selectedCategory: ''
    }
  },
  computed: {
    whatsappLink() {
      const jumlah = this.quantity * this.Produk.Harga

      const encodedProductName = encodeURIComponent(`${this.Produk.NamaProduk}`)
      const encodedProductPrice = encodeURIComponent(`${this.Produk.Harga}`)

      let message = `Nama: ${encodeURIComponent(
        this.personName
      )},%0APerusahaan: ${encodeURIComponent(
        this.companyName
      )},%0AMelakukan Pemesanan ${encodedProductName} Dengan Jumlah ${encodeURIComponent(
        this.quantity
      )} harga Rp${encodedProductPrice}%0ADeskripsi: ${encodeURIComponent(
        this.desc
      )}%0ATotal Yang Dibayar: ${jumlah}%0AMetode Pengiriman: ${this.selectedCategory}`

      if (this.selectedCategory === 'Delivery') {
        message += `%0AAlamat: ${encodeURIComponent(this.deliveryAddress)}`
      }

      return `https://wa.me/6281398396249?text=${message}`
    }
  },
  methods: {
    minusButton() {
      if (this.quantity > 1) {
        this.quantity--
      }
    },
    plusButton() {
      this.quantity++
    },
    calculateTotalPrice() {
      this.totalHarga = this.quantity * this.Produk.Harga
      console.log(this.totalHarga)
    },
    closeModal() {
      this.$emit('close')
    },
    handleDeliveryChange() {
      if (this.deliveryChecked) {
        this.pickupChecked = false
      }
    },
    handlePickupChange() {
      if (this.pickupChecked) {
        this.deliveryChecked = false
      }
    },
    toggleDelivery() {
      this.selectedCategory = this.selectedCategory === 'Delivery' ? '' : 'Delivery'
    },
    togglePickup() {
      this.selectedCategory = this.selectedCategory === 'Pick Up' ? '' : 'Pick Up'
    }
  },
  watch: {
    calculateTotalPrice: 'calculateTotalPrice'
  },
  created() {
    this.calculateTotalPrice()
  }
}
</script>
