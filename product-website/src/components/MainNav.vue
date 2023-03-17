<script setup>
import { RouterLink } from 'vue-router'

let drawerDisplayState = false
const drawer = () => {
  const draw = document.querySelector('#drawer')

  if (drawerDisplayState == false) {
    draw.classList.remove('hidden')
    drawerDisplayState = true
  } else {
    draw.classList.add('hidden')
    drawerDisplayState = false
  }
}
</script>
<template>
  <header
    class="sticky top-0 z-50 flex w-full items-center justify-between gap-4 bg-gray-900 py-2 px-4 sm:px-12 sm:pt-8"
  >
    <nav class="flex gap-4">
      <router-link to="/"
        ><img
          src="../images/disco.png"
          class="w-24 cursor-pointer rounded-lg opacity-80 sm:-mt-5 sm:w-32"
          alt="logo"
      /></router-link>

      <div class="hidden md:flex">
        <ul class="ml-4 flex gap-4 text-xl text-gray-200">
          <li>
            <RouterLink
              to="/"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >Home</RouterLink
            >
          </li>
          <li>
            <RouterLink
              to="/about"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >About</RouterLink
            >
          </li>
          <li>
            <RouterLink
              to="/pricing"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >Pricing</RouterLink
            >
          </li>
          <li>
            <RouterLink
              to="/contact"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >Contact</RouterLink
            >
          </li>
        </ul>
      </div>
    </nav>
    <div class="flex items-center justify-center gap-4 sm:-mt-3">
      <a class="hidden cursor-pointer sm:flex"
        ><img src="../images/facebook.png" class="w-8 bg-white" alt="facebook icon"
      /></a>
      <a class="hidden cursor-pointer sm:flex"
        ><img src="../images/discord.png" class="w-8 bg-white" alt="discord icon"
      /></a>
      <a class="hidden cursor-pointer sm:flex"
        ><img src="../images/github.png" class="w-8 bg-white" alt="github icon"
      /></a>
      <div class="drawer-content md:hidden">
        <!-- Page content here -->
        <label for="my-drawer" class="drawer-button btn-outline btn-sm btn" @click="drawer"
          >&#9776;</label
        >
      </div>
    </div>
  </header>

  <div class="drawer absolute z-40 hidden h-fit" id="drawer">
    <input id="my-drawer" type="checkbox" class="drawer-toggle" />

    <div class="drawer-side">
      <label for="my-drawer" class="drawer-overlay"></label>
      <ul class="menu w-full gap-4 overscroll-none bg-base-100 p-4 font-mono text-3xl text-white">
        <!-- Sidebar content here -->
        <li>
          <RouterLink
            to="/"
            class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >Home</RouterLink
          >
        </li>
        <li>
          <RouterLink
            to="/about"
            class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >About</RouterLink
          >
        </li>
        <li>
          <RouterLink
            to="/pricing"
            class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >Pricing</RouterLink
          >
        </li>
        <li>
          <RouterLink
            to="/contact"
            class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >Contact</RouterLink
          >
        </li>
        <li class="flex flex-row justify-evenly">
          <a class="hidden cursor-pointer sm:flex"
            ><img
              src="../images/facebook.png"
              class="w-8 cursor-pointer bg-white"
              alt="facebook icon"
          /></a>
          <a class="hidden cursor-pointer sm:flex"
            ><img
              src="../images/discord.png"
              class="w-8 cursor-pointer bg-white"
              alt="discord icon"
          /></a>
          <a class="hidden cursor-pointer sm:flex"
            ><img src="../images/github.png" class="w-8 cursor-pointer" alt="github icon"
          /></a>
        </li>
        <button class="btn-outline btn-secondary btn">Get Started</button>
      </ul>
    </div>
  </div>
</template>
