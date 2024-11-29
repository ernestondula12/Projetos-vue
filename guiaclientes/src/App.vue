<template>
    <div>
      <h1>Guia Clientes</h1>
      <input type="text" v-model="clienteErnesto.nome">
      <Cliente :nome="clienteErnesto.nome" :email="clienteErnesto.email" :idade="clienteErnesto.idade" :showIdade="true"/>
      <Cliente :nome="clienteKloriano.nome" :email="clienteKloriano.email" :idade="clienteKloriano.idade" :showIdade="false"/>
      <Cliente/>
      <Cliente/>
      <Cliente/>
      <Cliente/>
      <!--<Produto/>-->
    </div>
</template>

<script>
//Importando o meu componente cliente
import Cliente from './components/Cliente';
//import Produto from './components/Produto'
export default {
  name: 'App',
  data(){
    return {
      nomedoErnesto: "Ernesto Gime Ndula",
      clienteErnesto:{
          nome: "Ernesto Gimbi Ndula",
          email: "ernestondulandula@gmail.com",
          idade: 30
      },
      clienteKloriano:{
        nome: "Kloriano Luemba Brás",
        email: "kloriano@gmail.com",
        idade: 25
      }
    }    
  },
  components: {
    Cliente
  }
}
</script>

<style>
</style>
