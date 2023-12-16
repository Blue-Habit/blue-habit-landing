<template>
  <div>
    <Hero />
    <OurFocus />
    <VisionMision />
    <Products />
    <Teams />
    <Media />
  </div>
</template>

<script>
import Hero from "@/components/Hero";
import OurFocus from "@/components/OurFocus";
import VisionMision from "@/components/VisionMision";
import Products from "@/components/Products";
import Teams from "@/components/Teams";
import Media from "@/components/Media";
export default {
  components: {
    Hero,
    OurFocus,
    VisionMision,
    Products,
    Teams,
    Media
  },
};
</script>

<style scoped lang="scss"></style>
