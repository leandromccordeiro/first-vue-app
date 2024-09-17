<template>
    <div class="componente">
        <h1>
            Componente com dados
        </h1>
        <p>Nome: {{nomeProduto}} - {{codigoProduto}}</p>
    </div>
</template>

<script>
// options api
// export default{
//     data:function(){
//         return{
//              nomeProduto: "Caderno",
//              codigoProduto: "#321"
//         }
//     }
// }

//composition api
// export default {
//     setup:function() {
//         const nomeProduto = "Lápis"
//         const codigoProduto = "#789"
//         return {
//             nomeProduto, codigoProduto
//         }
//     }
// }

</script>

<script setup>
        const nomeProduto = "Lápis"
        const codigoProduto = "#789"
</script>