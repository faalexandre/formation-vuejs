<script setup>
import {ref} from 'vue'

const msg = ref('Mon premier destinataire')
</script>

<template>
  <main>
<h1>Message à: {{ msg.toUpperCase() }}</h1>
  </main>
</template>

<style scoped>


</style>