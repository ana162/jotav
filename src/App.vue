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
<button class="btn btn-primary" @click="incrementarContador">+</button>
<button class="btn btn-primary" @click="decrementarContador">-</button>
<p>Valor do contador é:{{ contador }}</p>
<hr>
<input v-model="nome" />
<input type="text" v-model="nome" />
<input type="password" v-model="senha" />
<input type="email" v-model="email" />
<input type="number" v-model="idade" />
<input type="text" v-model="nome" size="20" />
<input type="text" v-model="nome" maxlength="20" />
<input type="text" v-model="nome" minlength="3" />
<label for="aceitaTermos">Aceito os termos</label>
  <input type="checkbox" v-model="aceitaTermos" />
  <input type="checkbox" v-model="aceitaTermos" value="sim" />
  <label for="cores">Cores favoritas</label>
  <input type="text" v-model.number="idade" />
  <input type="text" v-model.lazy.number="idade" />
  <input type="text" v-model.trim.lazy.number="idade" />
  <input type="text" v-model="nome" autocomplete="on" />
  <input type="text" v-model="nome" readonly />
  <input type="text" v-model="nome" disabled />
  <input type="checkbox" v-model="cores" value="vermelho" /> Vermelho
  <input type="checkbox" v-model="cores" value="verde" /> Verde
  <input type="checkbox" v-model="cores" value="azul" /> Azul
  <label for="sexo">Sexo</label>
  <input type="text" v-model="nome" class="form-control" />
  <input type="text" v-model="nome" style="width: 200px" />
  <input type="text" v-model="nome" required />
  <input type="text" v-model.trim="nome" />
  <input type="text" v-model.lazy="nome" />
  <input type="text" v-model="nome" placeholder="Digite seu nome" />
  <input type="radio" v-model="sexo" value="masculino" /> Masculino
  <input type="radio" v-model="sexo" value="feminino" /> Feminino
  <label for="sexo">Sexo</label>
  <select v-model="sexo">
    <option value="masculino">Masculino</option>
    <option value="feminino">Feminino</option>
    <label for="cores">Cores favoritas</label>
  <select v-model="cores" multiple>
    <option value="vermelho">Vermelho</option>
    <option value="verde">Verde</option>
    <option value="azul">Azul</option>
  </select>
  <p>Cores favoritas: </p>
  </select>
  <p>Sexo: </p>
  <p>Sexo: </p>
  <p>Cores favoritas: </p>
  <p>Cores favoritas: </p>
  <p>Aceita os termos: </p>
  <p>Nome digitado é: </p> 
</template>
<textarea v-model="texto" rows="5" />
<textarea v-model="texto" cols="20" />
<textarea v-model="texto" />
  <p style="white-space: pre-line;">Texto digitado é: </p>
<style> 
/*estilos do componente baseado em css*/

</style>