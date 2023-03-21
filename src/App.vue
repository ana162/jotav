<script setup> 
//logica do componente
import { ref } from 'vue';

const contador = ref(0)
function incrementarContador(){ 
    contador.value++
}
function decrementarContador(){ 
    contador.value--
}
</script>


<template> 
<!--template do componente baseado em HTML-->
<button @click="incrementarContador">+</button>
<button @click="decrementarContador">-</button>
<p>Valor do contador é:{{ contador }}</p>
</template>

<style> 
/*estilos do componente baseado em css*/

</style>