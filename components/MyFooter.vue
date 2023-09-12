<template>
  <footer class="bg-primary w-full">
    <div class="max-w-screen-xl mx-auto p-4 md:py-8">
      <hr
        class="my-6 border-gray-200 opacity-40 sm:mx-auto dark:border-gray-700 lg:my-8"
      />
      <div class="grid lg:grid-cols-4 sm:grid-cols-1 gap-6">
        <div class="block">
          <a href="#" class="flex items-center mb-4 sm:mb-0">
            <img
              src="@/assets/img/Logo.png"
              class="h-8 mr-3"
              alt="bluhabit logo"
            />
          </a>
          <p class="text-sm text-white pt-5">
            Bluhabit 2023. All rights reserved
          </p>
        </div>
        <div class="block text-white">
          <h1 class="font-bold text-2xl pb-5">Business</h1>
          <p>+ 62 858 8256 8768</p>
          <p>support@bluhabit.com</p>
        </div>
        <div class="block text-white">
          <h1 class="font-bold text-2xl pb-5">Office</h1>
          <p>
            Jl. Nelayan Timur No. 1 Taman Sari, Jakarta Barat DKI Jakarta 11110
          </p>
        </div>
        <div class="block text-white">
          <h1 class="font-bold text-2xl pb-2">About us</h1>
          <h1 class="font-bold text-2xl pb-2">Vision</h1>
          <h1 class="font-bold text-2xl pb-2">Product</h1>
          <h1 class="font-bold text-2xl">Teams</h1>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MyFooter",
};
</script>

<style lang="scss" scoped></style>
