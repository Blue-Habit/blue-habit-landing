<template>
  <div class="w-auto">
    <img :src="imageSrc" class="w-full" alt="..." />
    <div class="p-4 bg-white">
      <h5 class="text-gray-700 mb-2">{{ name }}</h5>
      <p class="text-gray-900 mb-2">{{ position }}</p>
      <a :href="linkedinUrl">
        <img src="@/assets/img/img-linkedin.png" alt="" class="w-1/12" />
      </a>
    </div>
  </div>
</template>

<script setup lang="ts">

defineProps({
  name:{
    type:String,
    default:()=>""
  },
  position:{
    type:String,
    default:()=>""
  },
  linkedinUrl:{
    type:String,
    default:()=>""
  },
  imageSrc:{
    type:String,
    default:()=>""
  }
})
</script>

<style lang="scss" scoped></style>
