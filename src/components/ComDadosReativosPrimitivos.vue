<template>
    <div class="componente">
        <h1>Componentes com dados reativos</h1>
        <p>Nome: {{ nome }} | Idade: {{ idade }}</p>
        <button v-on:click="fazerAniversario">Fazer aniversário</button>
        <button @click="mudarNome">Mudar nome</button>
    </div>
</template>

<script setup>
import {ref} from "vue"
    const nome = ref("Leandro")
    const idade = ref(34)

    function fazerAniversario() {
        idade.value += 1
    }

    function mudarNome(){
        nome.value = "Cordeiro"
    }
</script>

