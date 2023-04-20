<template>
  <!-- Strutturare una card seguendo l'esempio in link -->
  <!-- https://v1.tailwindcss.com/components/cards -->
  <div class="card flex felx-col gap-4 ">
    {{ pokemon.name }}
    height: {{ pokemon_datail.height}}

    <div>
      <!-- cercare le abilità sotto pokemon_datail -->
      <span>Lista abilità:</span>
      <div>

      </div>
    </div>
    
  </div>
</template>


<script setup>
  const props = defineProps({
    pokemon: {
      type: Object
    }
  })

  const { data: pokemon_datail } = await useFetch(props.pokemon.url, { method: 'GET' })

</script>