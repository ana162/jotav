<script setup> 
//logica do componente
import { ref } from 'vue';
import { ref } from 'vue'

function handleFileUpload(e) {
  const target = e.target
  if (target && target.files) {
    const file = target.files[0]
    user.value.avatar = URL.createObjectURL(file)
  }
}
<img: src="user.avatar"/>
const user = ref({
  avatar: null
})
const contador = ref(0)
function incrementarContador(){ 
    contador.value++
}
function decrementarContador(){ 
    contador.value--
}
import { ref, computed } from 'vue'
const professor = ref({
    nome: 'Eduardo da Silva',
    disciplinas: [
        'Desenvolvimento Web II', 
        'Desenvolvimento de Aplicativos para Dispositivos Móveis',
    ]
})
import { ref } from 'vue'
const texto = ref('')
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
  <button @click="incrementar">{{ contador }} </button>
  <div>
        <h1>Professor</h1>
        <p>Nome: {{ professor.nome }}</p>
        <p>Possui disciplinas: {{ possuiDisciplinas }}</p>
    </div>
    <h1>Professor</h1>
<p>Nome: Eduardo da Silva</p>
<p>Possui disciplinas: Sim</p>
<h1>Professor</h1>
<p>Nome: Eduardo da Silva</p>
<p>Possui disciplinas: Não</p>
function possuiDisciplinas() {
    return professor.value.disciplinas.length > 0 ? 'Sim' : 'Não'
}
<div>
        <h1>Professor</h1>
        <p>Nome: {{ professor.nome }}</p>
        <p>Possui disciplinas: {{ possuiDisciplinas() }}</p>
    </div>
    <div>
        <input type="text" v-bind:value="texto" v-on:input="event => texto = event.target.value" />
        <p>Texto digitado: {{ texto }}</p>
    </div>
    <div>
        <input type="text" :value="texto" @input="event => texto = event.target.value" />
        <p>Texto digitado: {{ texto }}</p>
    </div>
    <div>
        <input type="text" v-model="texto" />
        <p>Texto digitado: {{ texto }}</p>
    </div>
    <input
    type="file"
    id="avatarField"
    @change="handleFileUpload($event)"
/>
</template>
<textarea v-model="texto" rows="5" />
<textarea v-model="texto" cols="20" />
<textarea v-model="texto" />
  <p style="white-space: pre-line;">Texto digitado é: </p>
<style> 
/*estilos do componente baseado em css*/

</style>