<template>
    <div>
        <h2>Nome da categoria: {{nome}}</h2>
        <h3>Descrição da categoria: {{descricao}}</h3>
        <h4>Duração do curso: {{duracao}}</h4>
    </div>
</template>

<script>
export default {
  data(){
    return{
    }
    },
    props:{
        nome: String,
        descricao: String,
        duracao: String,
        categoria: Object
    }
  }
</script>

<style scoped>

</style>