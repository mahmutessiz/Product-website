<script setup>
import { RouterLink } from 'vue-router'
</script>
<template>
  <div class="gradient flex min-h-screen items-center justify-center text-gray-300">
    <div class="container mx-auto flex flex-wrap items-center p-4">
      <div class="w-full flex justify-center p-4 text-center md:w-5/12">
        <img
          src="https://th.bing.com/th/id/OIP.IEoZIP96TEGo6-PAkfPwJgHaEo?pid=ImgDet&rs=1"
          alt="Not Found"
        />
      </div>
      <div
        class="flex w-full flex-col items-center justify-center p-4 text-center md:w-7/12 md:text-left"
      >
        <div class="text-6xl font-medium text-warning">404!</div>
        <div class="mb-4 text-xl font-medium md:text-3xl">Oops. This page has gone missing.</div>
        <div class="mb-8 text-lg">
          You may have mistyped the address or the page may have moved.
        </div>
        <div class="w-40 rounded border border-gray-400 p-4 text-center hover:scale-105">
          <RouterLink to="/">Go Home</RouterLink>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.gradient {
  background-image: linear-gradient(135deg, #0e0c12 35%, #252f41 100%);
}
</style>
