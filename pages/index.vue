<template>
  <div>
    <Hero />
    <OurFocus />
    <VisionMision />
    <Products />
    <Teams />
    <Footers />
  </div>
</template>

<script>
import Hero from "@/components/Hero";
import OurFocus from "@/components/OurFocus";
import VisionMision from "@/components/VisionMision";
import Products from "@/components/Products";
import Teams from "@/components/Teams";
import Footers from "@/components/Footers";
export default {
  components: {
    Hero,
    OurFocus,
    VisionMision,
    Products,
    Teams,
    Footers
  },
};
</script>

<style scoped lang="scss"></style>
