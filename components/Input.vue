<template>
  <div>
    <input :value="modelValue" 
    @input="$emit('update:modelValue', $event.target.value)"
    type="text" name="" id="" class="block border-2 border-gray-900 w-full p-2">
    <span class="bg-red-50 text-red-900">{{ messaggio }}</span>
  </div>
</template>

<script setup>
const props = defineProps({
  modelValue: String
})

const valore = ref('')
const messaggio = ref('')
const oggetto = reactive([ 1, 2, 3])

watch(valore, (newValue, oldValue) => {
  // quando valore è più lungo di 5 caratteri stampo un messaggio di errore
  if (newValue.length > 5)
    messaggio.value = 'Massimo 5 caratteri'
  else
    messaggio.value = ''

    oggetto.prop1
}, { immediate: true })

</script>

<style scoped>
.btn {
  padding: 1rem;
}
</style>