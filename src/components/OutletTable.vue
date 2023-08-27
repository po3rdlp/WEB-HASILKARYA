<template>
  <div class="overflow-x-auto">
    <table class="table table-zebra border rounded-lg">
      <!-- head -->
      <thead>
        <tr>
          <th>Kode Toko</th>
          <th>Alamat</th>
          <th>Jam Operasional</th>
          <th>Contact Person</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="data in Outlet" :key="data.di" class="border-b border-gray-300">
          <th class="font-bold">{{ data.kodeToko }}</th>
          <th>{{ data.alamat }}</th>
          <th>{{ data.jamOperasional }}</th>
          <th>{{ data.contactPerson }}</th>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import DataOutlet from '../assets/Data/DataOutlet.js'

export default {
  data() {
    return {
      Outlet: DataOutlet
    }
  }
}
</script>
