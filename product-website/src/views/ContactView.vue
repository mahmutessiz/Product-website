<template>
  <div class="w-full">
    <div class="h-96 bg-gradient-to-b from-rose-800 to-blue-600"></div>
    <div class="mx-auto mb-12 max-w-5xl px-6 sm:px-6 lg:px-8">
      <div class="-mt-72 w-full rounded bg-gray-900 p-8 shadow sm:p-12">
        <p class="text-center text-3xl font-bold leading-7 text-white">Contact</p>
        <form action="" method="post">
          <div class="mt-12 items-center md:flex">
            <div class="flex w-full flex-col md:w-1/2">
              <label class="font-semibold leading-none text-gray-300">Name</label>
              <input
                type="text"
                class="mt-4 rounded border-0 bg-gray-800 p-3 leading-none text-gray-50 focus:border-blue-700 focus:outline-none"
              />
            </div>
            <div class="mt-4 flex w-full flex-col md:ml-6 md:mt-0 md:w-1/2">
              <label class="font-semibold leading-none text-gray-300">Phone</label>
              <input
                type="email"
                class="mt-4 rounded border-0 bg-gray-800 p-3 leading-none text-gray-50 focus:border-blue-700 focus:outline-none"
              />
            </div>
          </div>
          <div class="mt-8 items-center md:flex">
            <div class="flex w-full flex-col">
              <label class="font-semibold leading-none text-gray-300">Subject</label>
              <input
                type="text"
                class="mt-4 rounded border-0 bg-gray-800 p-3 leading-none text-gray-50 focus:border-blue-700 focus:outline-none"
              />
            </div>
          </div>
          <div>
            <div class="mt-8 flex w-full flex-col">
              <label class="font-semibold leading-none text-gray-300">Message</label>
              <textarea
                type="text"
                class="mt-4 h-40 rounded border-0 bg-gray-800 p-3 text-base leading-none text-gray-50 focus:border-blue-700 focus:outline-none"
              ></textarea>
            </div>
          </div>
          <div class="flex w-full items-center justify-center">
            <button
              class="mt-9 rounded bg-blue-700 py-4 px-10 font-semibold leading-none text-white hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-700 focus:ring-offset-2"
            >
              Send message
            </button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>
