<template>
    <div class="componente">
        <h1>Componente que emite evento</h1>
        <p>{{ item }} (R${{ preco.toFixed(2) }})</p>
        <button @click="adicionar">Adicionar ao carrinho</button>
    </div>
</template>

<script setup>
    import { defineProps, defineEmits } from 'vue';

    const props = defineProps({
        item:String,
        preco:Number
    })

    const emite = defineEmits(["foiAdicionado"])

    function adicionar(){
        emite("foiAdicionado", props.preco)
    }
</script>