<script setup>
import { RouterLink } from 'vue-router'
</script>
<template>
  <header
    class="sticky top-0 z-50 flex w-full items-center justify-between gap-4 bg-gray-900 py-6 px-4 sm:px-12"
  >
    <nav class="flex gap-4">
      <img src="../../public/favicon.ico" class="cursor-pointer" alt="logo" />
      <div class="hidden md:flex">
        <ul class="ml-4 flex gap-4 text-xl text-gray-200">
          <li>
            <RouterLink
              to="/"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >Resouces</RouterLink
            >
          </li>
          <li>
            <RouterLink
              to="/"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >About</RouterLink
            >
          </li>
          <li>
            <RouterLink
              to="/"
              class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
              >Pricing</RouterLink
            >
          </li>
        </ul>
      </div>
    </nav>
    <div class="flex items-center justify-center gap-4">
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
        <label for="my-drawer" class="drawer-button btn-primary btn-outline btn">&#9776;</label>
      </div>
    </div>
  </header>

  <div class="drawer absolute z-20 h-fit md:hidden">
    <input id="my-drawer" type="checkbox" class="drawer-toggle" />

    <div class="drawer-side">
      <label for="my-drawer" class="drawer-overlay"></label>
      <ul class="menu w-full gap-4 overscroll-none bg-base-100 p-4 font-mono text-3xl text-white">
        <!-- Sidebar content here -->
        <li>
          <a href="#" class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >Resouces</a
          >
        </li>
        <li>
          <a href="#" class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >About</a
          >
        </li>
        <li>
          <a href="#" class="cursor-pointer transition-colors duration-300 hover:text-gray-400"
            >Pricing</a
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
