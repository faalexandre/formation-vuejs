<script setup>
import {ref} from 'vue'


//var
const msg = ref('Luanda terra dos braços aberto')
const count = ref(0)


//Func
const incrementCount = () => {
  count.value++
}

const resetCount = () => {
  count.value = 0
}

</script>

<template>
  <main>
<h1>{{ msg }}</h1>
<h2 :class="count < 10 ? 'green':  'red'"> Nombre = {{ count }}</h2>

<button @click="incrementCount">Incrémenter le nombre</button>
<button @click="resetCount">Réinitialiser le nombre</button>

  </main>
</template>

<style scoped>
.green {
  color: green;
}

.red {
  color: red;
}
</style>