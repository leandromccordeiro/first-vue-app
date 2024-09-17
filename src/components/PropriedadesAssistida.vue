<template>
    <div class="componente">
        <h1>Componente com propriedades assistidas</h1>
        <p>{{ idade }}</p>
        <label>Ano Nascimento</label>
        <input type="number" v-model="nascimento" min="1900"/>
        <label>Ano Atual:</label>
        <input type="number" v-model="anoAtual" min="2000"/>
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import { watchEffect } from 'vue';
    // import { watch } from 'vue';
    
    const nascimento = ref(1900)
    const anoAtual = ref(2000)
    const idade = ref(0)

    // watch(anoAtual, (ano)=> {
    //     idade.value = ano - nascimento.value
    // })

    // watch(nascimento, (ano)=>{
    //     idade.value = anoAtual.value - ano
    // })

</script>

<style scoped>
label {
    margin: 10px;
}
</style>