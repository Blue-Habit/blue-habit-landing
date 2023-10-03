<template>
  <div>
    <Hero />
    <OurFocus />
    <VisionMision />
    <Products />
  </div>
</template>

<script>
import Hero from "@/components/Hero";
import OurFocus from "@/components/OurFocus";
import VisionMision from "@/components/VisionMision";
import Products from "@/components/Products";

export default {
  components: {
    Hero,
    OurFocus,
    VisionMision,
    Products,
  },
};
</script>

<style scoped lang="scss"></style>
