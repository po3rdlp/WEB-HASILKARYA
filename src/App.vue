<template>
  <div class="absolute w-full top-0">
    <NavigationBar />
  </div>
  <div>
    <HomeView />
  </div>
</template>

<script setup>
import HomeView from './views/HomeView.vue'
import NavigationBar from './components/Navigationbar.vue'
</script>
