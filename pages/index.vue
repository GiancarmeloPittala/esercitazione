<template>
  <div>
    <Pokemon :pokemon="poke" v-for="poke of pokemon.results" :key="poke.name" />
  </div>
</template>

<script setup>
  const { data: pokemon } = await useFetch('https://pokeapi.co/api/v2/pokemon')
</script>