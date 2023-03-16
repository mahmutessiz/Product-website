<script setup>
import VanillaTilt from 'vanilla-tilt'
import { onMounted } from 'vue'

onMounted(() => {
  VanillaTilt.init(document.querySelectorAll('.tilt'), {
    max: 25,
    speed: 10000,
    axis: 'x'
  })
})
</script>

<template>
  <div class="mt-24 grid w-full place-items-center">
    <h2 class="text-3xl font-bold text-gray-300 sm:text-5xl">Some cool stuf</h2>
  </div>

  <!-- image galery -->
  <section class="flex w-full justify-center">
    <div
      class="mt-12 flex h-fit max-w-[52rem] flex-wrap items-center justify-center gap-4 py-8 px-4 md:grid md:grid-cols-12 md:grid-rows-6 md:place-items-center md:gap-0"
    >
      <div class="tilt p-1 md:col-span-3 md:row-span-2 md:w-1/2 md:min-w-[12rem] md:p-2">
        <img
          alt="gallery"
          class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500"
          src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(70).webp"
        />
      </div>
      <div class="tilt p-1 md:col-span-3 md:row-span-2 md:w-1/2 md:min-w-[12rem] md:p-2">
        <img
          alt="gallery"
          class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500"
          src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(72).webp"
        />
      </div>
      <div class="tilt p-1 md:col-span-6 md:row-span-4 md:w-1/2 md:min-w-[23rem] md:p-2">
        <img
          alt="gallery"
          class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500"
          src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(73).webp"
        />
      </div>
      <div class="tilt w-full p-1 md:col-span-6 md:row-span-4 md:min-w-[23rem] md:p-2">
        <img
          alt="gallery"
          class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500"
          src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(74).webp"
        />
      </div>
      <div class="tilt p-1 md:col-span-3 md:row-span-2 md:w-1/2 md:min-w-[12rem] md:p-2">
        <img
          alt="gallery"
          class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500"
          src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(75).webp"
        />
      </div>
      <div class="tilt p-1 md:col-span-3 md:row-span-2 md:w-1/2 md:min-w-[12rem] md:p-2">
        <img
          alt="gallery"
          class="block h-full w-full rounded-lg object-cover object-center transition-all duration-500"
          src="https://tecdn.b-cdn.net/img/Photos/Horizontal/Nature/4-col/img%20(77).webp"
        />
      </div>
    </div>
  </section>
</template>
