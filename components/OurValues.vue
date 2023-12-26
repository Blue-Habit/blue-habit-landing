<template>
    <div class="bg-gray-100 py-16">
        <div class="grid lg:grid-cols-2 sm:grid-cols-1 lg:px-16 sm:px-5 justify-between">
            <div class="flex flex-col">
                <h1 class="text-primary text-2xl font-bold mb-5">Our Values</h1>
                <h1 class="text-5xl font-bold mb-5">Nurturing Growth and Excellence</h1>
                <p class="text-gray-700">We prioritize team development through learning and growth spaces. Our nurturing
                    culture celebrates personal and professional growth, while adhering to industry project management
                    standards.</p>
            </div>
            <div class="flex flex-col gap-7 w-full">
                <div v-for="(value, index) in values" :key="index" class="bg-white w-full p-5">
                    <img :src="value.icon" :alt="`${value.title} Icon`" class="w-1/12 mb-3">
                    <h1 class="text-xl font-bold mb-3">{{ value.title }}</h1>
                    <p class="text-gray-700">{{ value.description }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import growth from "@/assets/img/icon-growth.png";
import supportive from "@/assets/img/icon-supportive.png";
import empowering from "@/assets/img/icon-empowering.png";

const values = ref([
    {
        title: "Learning and Growth Space",
        icon: growth,
        description:
            "Our team's growth is paramount. We've established a learning space for acquiring new skills and insights, while our growth space focuses on personal development.",
    },
    {
        title: "Supportive Culture",
        icon: supportive,
        description:
            "Our culture revolves around support and rewards. We've created an environment where personal and professional development are valued and encouraged.",
    },
    {
        title: "Industry-Leading Project Management",
        icon: empowering,
        description:
            "In our pursuit of excellence, our project management practices stand up to industry standards.",
    },
]);
</script>

<style lang="scss" scoped></style>
