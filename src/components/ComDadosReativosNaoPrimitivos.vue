<template>
    <div class="componente">
        <h1>Componentes com dados reativos NÃO PRIMITIVOS</h1>
        <p>Nome: {{ pessoa.nome }} | Idade: {{ pessoa.idade }}</p>
        <button v-on:click="fazerAniversario">Fazer aniversário</button>
        <button @click="mudarNome">Mudar nome</button>
    </div>
</template>

<script setup>
import {reactive} from "vue"
const pessoa = reactive({nome:"Leandro", idade:34})

function fazerAniversario() {
    pessoa.idade += 1
}

function mudarNome(){
    pessoa.nome = "Cordeiro"
}
</script>

