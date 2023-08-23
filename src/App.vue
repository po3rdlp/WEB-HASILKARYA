<template>
  <div class="absolute w-full top-0 z-10">
    <NavigationBar />
  </div>
  <div>
    <RouterView />
  </div>
  <div>
    <FooterBar />
  </div>
</template>

<script setup>
import NavigationBar from './components/Navigationbar.vue'
import FooterBar from './components/FooterBar.vue'
</script>
