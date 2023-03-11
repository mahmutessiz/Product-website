<script setup>
import MainNav from './components/MainNav.vue'
import FooterSection from './components/FooterSection.vue'
import { RouterView } from 'vue-router'
</script>

<template>
  <MainNav />
  <RouterView />
  <FooterSection />
</template>
