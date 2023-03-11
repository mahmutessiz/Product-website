<template>
  <section class="mt-12 mb-12 flex w-full flex-col items-center justify-center">
    <h2 class="py-4 text-center text-3xl font-bold text-gray-300 underline">
      Product's pros & cons
    </h2>
    <div class="flex w-2/3 flex-col">
      <div class="overflow-x-auto sm:-mx-6 lg:-mx-8">
        <div class="inline-block min-w-full py-2 sm:px-6 lg:px-8">
          <div class="overflow-hidden">
            <table class="min-w-full text-center text-sm font-light">
              <thead class="border-b font-medium dark:border-neutral-500">
                <tr>
                  <th scope="col" class="px-6 py-4">Your product</th>
                  <th scope="col" class="px-6 py-4">Others</th>
                  <th scope="col" class="px-6 py-4">Others</th>
                </tr>
              </thead>
              <tbody>
                <tr class="border-b dark:border-neutral-500">
                  <td class="whitespace-nowrap px-6 py-4">✅</td>
                  <td class="whitespace-nowrap px-6 py-4">❎</td>
                  <td class="whitespace-nowrap px-6 py-4">❎</td>
                </tr>
                <tr class="border-b dark:border-neutral-500">
                  <td class="whitespace-nowrap px-6 py-4">✅</td>
                  <td class="whitespace-nowrap px-6 py-4">❎</td>
                  <td class="whitespace-nowrap px-6 py-4">❎</td>
                </tr>
                <tr class="border-b dark:border-neutral-500">
                  <td class="whitespace-nowrap px-6 py-4">✅</td>
                  <td class="whitespace-nowrap px-6 py-4">❎</td>
                  <td class="whitespace-nowrap px-6 py-4">❎</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
