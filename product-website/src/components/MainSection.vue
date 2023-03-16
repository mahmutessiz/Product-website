<script setup>
import ProductsSection from './ProductsSection.vue'
import CompareOthersSection from './CompareOthersSection.vue'
import UtilitiesSection from './UtilitiesSection.vue'
import GetInTouchSection from './GetInTouchSection.vue'
import TestimonialSection from './TestimonialSection.vue'
</script>

<template>
  <main class="relative grid h-screen w-full place-items-center px-12">
    <video
      playsinline
      autoplay
      muted
      loop
      poster="../images/facebook.png"
      class="absolute top-0 w-full opacity-20 md:hidden"
    >
      <source src="../images/phone_bg.webm" type="video/webm" />
      Your browser does not support the video tag.
    </video>

    <video
      playsinline
      autoplay
      muted
      loop
      poster="../images/facebook.png"
      class="absolute -z-10 hidden w-full md:block"
    >
      <source src="../images/site_bg.webm" type="video/webm" />
      Your browser does not support the video tag.
    </video>
    <div class="z-10 md:w-1/2">
      <h1 class="text-center font-serif text-3xl font-bold leading-snug text-gray-200 sm:text-6xl">
        <span class="bg-gradient-to-r from-rose-400 to-purple-500 bg-clip-text text-transparent">
          Add your website's motto in here
        </span>
      </h1>
      <p class="mt-12 text-center text-gray-300 sm:text-xl">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere, consequatur at. Soluta
        laboriosam qui eaque cumque cum ipsa quibusdam nostrum expedita aliquam iste assumenda,
        placeat quae voluptatum eos officiis aspernatur!
      </p>
      <div class="flex w-full justify-center">
        <button class="btn-outline btn-warning btn mt-9 hover:scale-105">Try for free</button>
      </div>
    </div>
  </main>
  <div class="m-auto mt-12 w-2/3 max-w-[52rem] text-center" id="sponsor-div">
    <span class="text-2xl text-gray-200"
      >Sponsors
      <hr />
    </span>
    <ul class="mt-4 flex flex-wrap justify-center gap-6 p-9">
      <li class="border-b border-warning shadow-sm shadow-slate-500">
        <img
          src="https://picsum.photos/100/60/"
          class="transition-transform duration-300 hover:scale-105"
          alt=""
        />
      </li>
      <li class="border-b border-warning shadow-sm shadow-slate-500">
        <img
          src="https://picsum.photos/100/64/"
          class="transition-transform duration-300 hover:scale-105"
          alt=""
        />
      </li>
      <li class="border-b border-warning shadow-sm shadow-slate-500">
        <img
          src="https://picsum.photos/100/63/"
          class="transition-transform duration-300 hover:scale-105"
          alt=""
        />
      </li>
      <li class="border-b border-warning shadow-sm shadow-slate-500">
        <img
          src="https://picsum.photos/100/62/"
          class="transition-transform duration-300 hover:scale-105"
          alt=""
        />
      </li>
      <li class="border-b border-warning shadow-sm shadow-slate-500">
        <img
          src="https://picsum.photos/100/61/"
          class="transition-transform duration-300 hover:scale-105"
          alt=""
        />
      </li>
    </ul>
  </div>

  <ProductsSection />
  <UtilitiesSection />
  <CompareOthersSection />
  <TestimonialSection />
  <GetInTouchSection />
</template>
