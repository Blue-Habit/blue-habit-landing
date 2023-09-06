<template>
  <div class="products mx-auto py-9">
    <h1 class="text-primary text-xl lg:px-16 sm:px-5">Our Products</h1>
    <h1 class="text-5xl text-gray-900 font-bold pt-3 lg:px-16 sm:px-5">
      Throught Collaborations,
      <br />We Produce Best Solutions
    </h1>
    <div class="grid lg:grid-cols-2 sm:grid-cols-1 lg:px-16 sm:px-5 gap-5">
      <div class="w-auto">
        <img src="@/assets/img/img-gawean.png" class="w-full" alt="..." />
        <div class="p-4">
          <h5 class="text-gray-700 mb-2">Gawean</h5>
          <p class="text-gray-900">
            Task Management app for Elevating Productivity Habits for
            Individuals and Teams
          </p>
        </div>
      </div>
      <div class="w-auto">
        <img src="@/assets/img/img-budgetku.png" class="w-full" alt="..." />
        <div class="p-4">
          <h5 class="text-gray-700 mb-2">Budgetku</h5>
          <p class="text-gray-900">
            Personal financial recording app with budget settings and financial
            planning for better habits
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Products",
};
</script>

<style lang="scss" scoped></style>
