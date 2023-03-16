<script setup>
import ProductsSection from './ProductsSection.vue'
import CompareOthersSection from './CompareOthersSection.vue'
import UtilitiesSection from './UtilitiesSection.vue'
import GetInTouchSection from './GetInTouchSection.vue'
import TestimonialSection from './TestimonialSection.vue'
import SponsorSection from './SponsorSection.vue'
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
      <p class="mt-12 text-left text-gray-300 sm:pl-6 sm:text-xl">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere, consequatur at. Soluta
        laboriosam qui eaque cumque cum ipsa quibusdam nostrum expedita aliquam iste assumenda,
        placeat quae voluptatum eos officiis aspernatur!
      </p>
      <div class="flex w-full justify-center">
        <button class="btn-outline btn-warning btn mt-9 hover:scale-105">Try for free</button>
      </div>
    </div>
  </main>

  <ProductsSection />
  <UtilitiesSection />
  <CompareOthersSection />
  <TestimonialSection />
  <SponsorSection />
  <GetInTouchSection />
</template>
