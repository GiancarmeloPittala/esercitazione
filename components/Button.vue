<template>
  <button class="border border-gray-900 rounded-lg transition-colors"
  :class="[colorClasses[color], sizeClasses[dim]]">

    <slot name="label"> Api call </slot>
    <slot></slot>
    
  </button>
</template>

<script setup>

  //componete creato e rendirizzato 
 onMounted(() => {

 })

 // il componente è stato distrutto 
 onUnmounted(() => {
  
 })


const props = defineProps({
  color: String,
  dim: String,
  label: String
})


const colorClasses = {
  nero: 'hover:bg-gray-900 hover:text-gray-50',
  rosso: 'hover:bg-red-900 hover:text-red-50'
}

const sizeClasses = {
  large: 'py-1.5 px-3',
  small: 'py-1 px-2'
}

</script>

<style scoped>
 .btn{
  padding: 1rem;
 }
</style>