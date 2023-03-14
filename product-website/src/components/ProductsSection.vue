<script setup>
import VanillaTilt from 'vanilla-tilt'
import { onMounted } from 'vue'

onMounted(() => {
  VanillaTilt.init(document.querySelectorAll('.tilt'), {
    max: 25,
    speed: 400,
    scale: 1.1
  })
})
</script>

<template>
  <div class="mt-12 mb-8 grid w-full place-items-center">
    <h2 class="text-3xl font-bold text-gray-300 underline">Some cool stuf</h2>
  </div>

  <!-- image galery -->
  <section class="overflow-hidden text-neutral-700">
    <div class="container mx-auto px-5 py-2 lg:px-32 lg:pt-24">
      <div class="-m-1 flex flex-wrap md:-m-2">
        <div class="flex w-1/2 flex-wrap">
          <div class="tilt w-1/2 p-1 md:p-2">
            <img
              alt="gallery"
              class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500 hover:scale-105"
              src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(70).webp"
            />
          </div>
          <div class="tilt w-1/2 p-1 md:p-2">
            <img
              alt="gallery"
              class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500 hover:scale-105"
              src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(72).webp"
            />
          </div>
          <div class="tilt w-full p-1 md:p-2">
            <img
              alt="gallery"
              class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500 hover:scale-105"
              src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(73).webp"
            />
          </div>
        </div>
        <div class="flex w-1/2 flex-wrap">
          <div class="tilt w-full p-1 md:p-2">
            <img
              alt="gallery"
              class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500 hover:scale-105"
              src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(74).webp"
            />
          </div>
          <div class="tilt w-1/2 p-1 md:p-2">
            <img
              alt="gallery"
              class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500 hover:scale-105"
              src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(75).webp"
            />
          </div>
          <div class="tilt w-1/2 p-1 md:p-2">
            <img
              alt="gallery"
              class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500 hover:scale-105"
              src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(77).webp"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
