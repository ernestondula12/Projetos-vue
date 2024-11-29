<template>
    <div id="cliente">
        <h4>Nome: {{nome}}</h4>
        <hr>
        <p>Email: {{email}}</p>
        <hr />
        <p v-show="showIdade == true ">Idade:{{idade}}</p>
    </div>
</template>

<!--A minha lógica onde vou poder definir variaveis, metodos e tantos outros elementos-->
<script>
    export default{
        data(){
            return {
            }
        },
        props: {
            nome: String,
            email: String,
            idade: Number,
            cliente: Object,
            showIdade: Boolean
        }
    }
</script>

<!--A area onde vou poder trabalhar com a estilização dos meus componentes-->
<style scoped>
    #cliente{
        color: blue;
        background-color: aqua;
        max-width: 600px;
        height: 170px;
        border-radius: 10px;
        padding: 13px;
        margin-top: 10px;
        margin-left: 20px;
    }
</style>
