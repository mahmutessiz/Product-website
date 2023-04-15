<script setup>
import VanillaTilt from 'vanilla-tilt'
import { RouterLink } from 'vue-router'
import { onMounted } from 'vue'

onMounted(() => {
  VanillaTilt.init(document.querySelector('.tilt-getintouch'), {
    max: 25,
    speed: 10000,
    scale: 1.1
  })
})
</script>
<template>
  <section class="flex w-full justify-center bg-slate-900 pt-24 pb-24">
    <div class="tilt-getintouch card w-1/2 max-w-[52rem] bg-slate-800 shadow-xl">
      <figure class="py-4 px-2 sm:px-10 sm:pt-10">
        <img src="https://picsum.photos/500/200/" alt="Random photo" class="rounded-xl" />
      </figure>
      <div class="card-body items-center text-center text-xl text-gray-200">
        <p>Ask anythink you want about us.</p>
        <div class="card-actions mt-8">
          <RouterLink to="/contact"
            ><button class="btn-outline btn-warning btn hover:scale-105">
              Get in touch
            </button></RouterLink
          >
        </div>
      </div>
    </div>
  </section>
</template>
