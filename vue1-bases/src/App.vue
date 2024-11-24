<script setup>
import {ref} from 'vue'

// var
let msg = ref('luanda','Modifier le nombre')
const count = ref(0)
const changeMsg = ()=>{
  msg.value = 'Faustino'
}

const resetcount = ()=>{
  count.value = 0
}

</script>

<template>
  <main>
<h1 @click="changeMsg">{{ msg }}</h1>
<h2>Nombre = {{ count }}</h2>
<button @click="count++">Incrémenter le nombre</button>
<button @click="resetcount">Réinitialiser le nombre</button>
  </main>
</template>

<style scoped>
h1:hover {
  cursor: pointer;
}

</style>