<template>
    <div class="teams mx-auto pt-9">
        <h1 class="text-primary text-xl lg:px-16 sm:px-5">Media</h1>
        <div class="grid lg:grid-cols-2 sm:grid-cols-1 mb-16">
            <h1 class="text-5xl text-gray-900 font-bold pt-3 lg:px-16 sm:px-5">
                Proudly <br> Featured In
            </h1>
            <div>
                <img src="@/assets/img/cta-img2.png" alt="">
            </div>
        </div>
        <div class="grid lg:grid-cols-2 sm:grid-cols-1 lg:px-16 sm:px-5 pt-6">
            <img src="@/assets/img/cta-img.png" alt="" class="w-3/5">
            <div class="d-flex flex-col lg:pr-20">
                <h1 class="text-5xl font-bold pb-2 pt-3">Start Making a</h1>
                <h1 class="text-5xl font-bold pb-9">Difference Today</h1>
                <p class="text-gray-700 pb-9">Empower yourself with the knowledge and tools to create a brighter financial
                    future. Take the first step towards enhancing your financial literacy, embracing positive habits, and
                    unlocking a world of possibilities.</p>
                <button class="bg-primary px-3 py-2 text-white rounded-lg">Button Label</button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "Cta"
}
</script>