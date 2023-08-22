<template>
  <div class="absolute w-full top-0 z-50">
    <NavigationBar />
  </div>
  <div>
    <HomeView />
  </div>
  <div>
    <FooterBar />
  </div>
</template>

<script setup>
import HomeView from './views/HomeView.vue'
import NavigationBar from './components/Navigationbar.vue'
import FooterBar from './components/FooterBar.vue'
</script>
