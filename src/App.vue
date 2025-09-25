<template>
  <div class="max-w-7xl mx-auto py-4 sm:py-6 md:py-8 lg:py-12 px-2 sm:px-4 md:px-6 lg:px-8">

    <div class="flex justify-center mb-4 sm:mb-6">
      <PokemonSearch @search="searchPokemon" />
    </div>

    <div v-if="loading" class="flex justify-center mb-4 sm:mb-6">
      <div class="animate-spin rounded-full h-8 w-8 sm:h-10 sm:w-10 md:h-12 md:w-12 border-t-2 border-blue-500 border-b-2"> </div>
    </div>

    <div v-if="!loading && filteredPokemons.length === 0" class="text-center py-6 sm:py-8">
      <p class="text-base sm:text-lg md:text-xl text-gray-500 px-4">Aucun pokemon trouvé pour votre recherche</p>
    </div>

    <Transition name="fade" mode="out-in">
      <PokemonList v-if="!loading && filteredPokemons.length > 0" :pokemons="filteredPokemons">
        <template #default="{ pokemon }">
          <PokemonCard :pokemon="pokemon" />
        </template>
      </PokemonList>
    </Transition>

  </div>
</template>



<script setup>
import { ref, onMounted, computed } from 'vue'
import PokemonSearch from './components/PokemonSearch.vue'
import PokemonList from './components/PokemonList.vue'
import PokemonCard from './components/PokemonCard.vue'

const pokemons = ref([])
const searchQuery = ref('')
const loading = ref(true)

onMounted(async () => {
  try {
    const response = await fetch('https://pokebuildapi.fr/api/v1/pokemon')
    
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`)
    }
    
    const data = await response.json()
    pokemons.value = data
    loading.value = false
  } catch (error) {
    console.error('Error fetching data:', error)
    loading.value = false
  }
});

const filteredPokemons = computed(() => {
  if (!searchQuery.value) return pokemons.value
  return pokemons.value.filter((pokemon) => pokemon.name.toLowerCase().includes(searchQuery.value.toLowerCase()))
})


const searchPokemon = (query) => {
  searchQuery.value = query
}

</script>



<style>

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

</style>