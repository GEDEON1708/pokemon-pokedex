<template>
    <div class="rounded-lg border border-gray-300 p-2 sm:p-3 md:p-4 text-center bg-white shadow-md hover:shadow-lg transition-all duration-300 hover:border-blue-500 h-full flex flex-col">
        <img :src="pokemon.image" :alt="pokemon.name" class="w-16 h-16 sm:w-20 sm:h-20 md:w-24 md:h-24 mx-auto transition-transform duration-500 hover:rotate-3 hover:scale-110 flex-shrink-0">

        <h2 class="text-sm sm:text-base md:text-lg lg:text-xl font-bold mt-1 sm:mt-2 text-gray-800 leading-tight">{{ pokemon.name }}</h2>

        <div class="mt-1 sm:mt-2 space-y-0.5 sm:space-y-1 flex-grow flex flex-col justify-end">
            <p class="text-xs sm:text-sm md:text-base text-gray-700 transition-all duration-200 hover:text-blue-500"> ⚡PV:{{ pokemon.stats.HP }}</p>
            <p class="text-xs sm:text-sm md:text-base text-gray-700 transition-all duration-200 hover:text-rose-500"> 🗡️ ATK:{{ pokemon.stats.attack }}</p>
            <p class="text-xs sm:text-sm md:text-base text-gray-700 transition-all duration-200 hover:text-green-500"> 🛡️ DEF:{{ pokemon.stats.defense }}</p>
        </div>
        
    </div>

</template>


<script setup>

import { defineProps } from "vue";

defineProps({
    pokemon: Object,
});

</script>


<style>

</style>