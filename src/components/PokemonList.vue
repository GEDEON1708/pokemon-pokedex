<template>
    <TransitionGroup name="list" tag="div" class="grid grid-cols-1 xs:grid-cols-2 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 2xl:grid-cols-6 gap-2 sm:gap-3 md:gap-4 p-2 sm:p-3 md:p-4 lg:p-5 auto-rows-fr">
        <div v-for="pokemon in pokemons" :key="pokemon.id"
            class="transform hover:scale-105 transition-all duration-200">
            <slot :pokemon="pokemon"></slot>
        </div>
    </TransitionGroup>
</template>

<script setup>
import { defineProps } from "vue";

defineProps({
    pokemons: Array,
});
</script>

<style>
.list-move,
.list-enter-active,
.list-leave-active {
    transition: all 0.3s ease;
}

.list-enter-from,
.list-leave-to {
    opacity: 0;
    transform: translateY(20px);
}
</style>
