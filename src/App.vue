<script> 
// Será apresentado a seguir
</script>

<template> 
<button @click="incrementarcontador">incrementar</button>
<button @click="decrementarcontador">decrementar</button>
<p> Valor do contador é: {{ contador }}</p>
</template>
<style scoped>
button{
    font-weight: bold;
}
</style>