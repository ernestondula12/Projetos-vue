<template>
      <div>
          <Categorias :nome="categoriaWeb.nome" :descricao="categoriaWeb.descricao" :duracao="categoriaWeb.duracao"/>
      </div>
</template>

<script>

import Categorias from './components/Categorias'

export default {
  name: 'App',
    data(){
        return {
          nomeDaCategoria: "Desenvolvimento Web",
          categoriaWeb:{
              nome: "Desenvolvimento Mobile",
              descricao: "Desenvolvimento web seguro",
              duracao: 20
          }
        }
    },
  components: {
    Categorias
  }
}
</script>

<style>

  .titulo{
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-weight: bold;
    font-family: "Trebuchet MS", Arial, Helvetica, sans-serif;
    text-decoration: underline;
  }

</style>
