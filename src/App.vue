<template>
  <div class="absolute w-full top-0 z-20">
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
import NavigationBar from '@/components/NavigationBar.vue'
import FooterBar from './components/FooterBar.vue'
</script>
