<template>
  <div>
    <Hero />
    <OurFocus />
    <VisionMision />
    <Products />
    <Teams />
    <Cta />
  </div>
</template>

<script>
import Hero from "@/components/Hero";
import OurFocus from "@/components/OurFocus";
import VisionMision from "@/components/VisionMision";
import Products from "@/components/Products";
import Teams from "@/components/Teams";
import Cta from "@/components/Cta";
export default {
  components: {
    Hero,
    OurFocus,
    VisionMision,
    Products,
    Teams,
    Cta
  },
};
</script>

<style scoped lang="scss"></style>
