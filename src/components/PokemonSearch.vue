<template>

    <div class="w-full max-w-sm sm:max-w-md md:max-w-lg lg:max-w-xl relative">
        <Transition name="slide">
            <input type="text" v-model="query" @input="emitSearch" placeholder="🔎 Recherche un Pokemon" class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-md mb-3 sm:mb-4 md:mb-5 text-sm sm:text-base focus:outline-none focus:ring-2 focus:ring-blue-500 transition-all duration-300 hover:shadow-md placeholder:text-xs sm:placeholder:text-sm"></input>
        </Transition>
    </div>

</template>


<script setup>
import {ref} from 'vue'

const query = ref('')
const emit = defineEmits([ 'search'])


const emitSearch=()=>{
    emit("search", query.value)
}

</script>


<style>

.slide-enter-active{
    transition: all 0.4s ease-in-out;
}

.slide-leave-active{
    transition: all 0.3s ease-in-out;
}

.slide-enter-from{
    transform: translateY(-20px);
    opacity: 0;
}

.slide-leave-to{
    transform: translateY(20px);
    opacity: 0;
}

</style>