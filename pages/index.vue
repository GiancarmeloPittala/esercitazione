<template>
  <div>
    <Input v-model="testo" />
    {{ testo }}
    <Button color="nero" dim="large">
      <template v-slot:label>
       label
      </template>
      <p>
        testo
      </p>
    </Button>
    <Button color="rosso" dim="small">
      secondo testo
    </Button>

    <Button color="nero">
      tttt
    </Button>

    <Button color="rosso">
      ttt
    </Button>

  </div>
</template>

<script setup>
const testo = ref("")
</script>