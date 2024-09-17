<template>
    <div class="componente">
        <h1>Componente com propriedades computadas</h1>
        <p>{{ idade }}</p>
        <label>Ano Nascimento</label>
        <input type="number" v-model="nascimento" min="1900"/>
        <label>Ano Atual:</label>
        <input type="number" v-model="anoAtual" min="2000"/>
    </div>
</template>

<script setup>
    import { ref, computed } from 'vue';
    const nascimento = ref(1900)
    const anoAtual = ref(2000)
    const idade = computed(()=>{
        return anoAtual.value - nascimento.value 
    })
</script>

<style scoped>
label {
    margin: 10px;
}
</style>