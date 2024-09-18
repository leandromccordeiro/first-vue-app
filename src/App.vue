<script setup>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import ComDados from "./components/ComDados.vue"
import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue";
import DataBinding from "./components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
import EscutaEvento from "./components/EscutaEvento.vue";
import PropriedadesComputadas from "./components/PropriedadesComputadas.vue";
import PropriedadesAssistida from "./components/PropriedadesAssistida.vue";
import RenderizacaoCondicional from "./components/RenderizacaoCondicional.vue";
</script>

<template>
  <header>Vue</header>
  <RenderizacaoCondicional nome="Thayane" :qtd-cachorros="1"/>
  <PropriedadesAssistida/>
  <PropriedadesComputadas/>
  <EscutaEvento/>
  <ComProps item="Borracha" :preco="2.50"/>
  <DataBinding/>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <ComDados/>
  <PrimeiroComponente/>
</template>

<style scoped>
</style>
