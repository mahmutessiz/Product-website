<script setup></script>
<template>
  <header class="flex w-full items-center justify-between gap-4 bg-black py-6 px-4 sm:px-12">
    <nav class="flex gap-4">
      <img src="../../public/favicon.ico" alt="logo" />
      <div class="hidden md:flex">
        <ul class="ml-4 flex gap-4 text-3xl text-gray-200">
          <li><a>Docs</a></li>
          <li><a>Showcase</a></li>
          <li><a>Resouces</a></li>
          <li><a>About</a></li>
          <li><a>Blog</a></li>
        </ul>
      </div>
    </nav>
    <div class="flex items-center justify-center gap-4 text-3xl">
      <a class="hidden sm:flex">T</a>
      <a class="hidden sm:flex">D</a>
      <a class="hidden sm:flex">G</a>
      <div class="drawer-content md:hidden">
        <!-- Page content here -->
        <label for="my-drawer" class="drawer-button btn-primary btn-outline btn">&#9776;</label>
      </div>
    </div>
  </header>

  <div class="drawer fixed z-50 md:hidden">
    <input id="my-drawer" type="checkbox" class="drawer-toggle" />

    <div class="drawer-side">
      <label for="my-drawer" class="drawer-overlay"></label>
      <ul class="menu w-full gap-4 bg-base-100 p-4 font-mono text-3xl text-white">
        <!-- Sidebar content here -->
        <li><a>Docs</a></li>
        <li><a>Showcase</a></li>
        <li><a>Resouces</a></li>
        <li><a>About</a></li>
        <li><a>Blog</a></li>
        <li class="flex flex-row justify-evenly">
          <a>T</a>
          <a>D</a>
          <a>G</a>
        </li>
        <button class="btn-outline btn-secondary btn">Get Started</button>
      </ul>
    </div>
  </div>
</template>
