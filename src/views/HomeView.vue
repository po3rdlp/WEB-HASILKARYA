<template>
  <div>
    <SectionIntro />
  </div>
  <div id="about">
    <SectionBackground />
  </div>
  <div id="products">
    <SectionProducts />
  </div>
  <div>
    <SectionFindUs />
  </div>
</template>

<script setup>
import SectionIntro from '../components/SectionHome/SectionIntro.vue'
import SectionBackground from '../components/SectionHome/SectionBackground.vue'
import SectionProducts from '../components/SectionHome/SectionProducts.vue'
import SectionFindUs from '../components/SectionHome/SectionFindUs.vue'
</script>
