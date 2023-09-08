<template>
  <div>
    <Hero />
    <OurFocus />
    <VisionMision />
    <Products />
    <Teams />
  </div>
</template>

<script>
import Hero from "@/components/Hero";
import OurFocus from "@/components/OurFocus";
import VisionMision from "@/components/VisionMision";
import Products from "@/components/Products";
import Teams from "../components/Teams";
export default {
  components: {
    Hero,
    OurFocus,
    VisionMision,
    Products,
    Teams,
  },
};
</script>

<style lang="scss" scoped></style>
