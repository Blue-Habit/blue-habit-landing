<template>
  <div>
    <Hero />
    <OurFocus />
    <VisionMision />
  </div>
</template>

<script>
import Hero from "@/components/Hero";
import OurFocus from "@/components/OurFocus";
import VisionMision from "@/components/VisionMision";
import OurFocus from "../components/OurFocus.vue";

export default {
  components: {
    Hero,
    OurFocus,
    VisionMision,
  },
};
</script>

<style lang="scss" scoped></style>
