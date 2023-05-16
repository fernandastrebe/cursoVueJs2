<template>
  <div id="app">
    <h1>Bem-vindo ao meu primeiro projeto!</h1>
    <p>Componente pai: {{nome}}</p>
    <button @click="entrar">Entrar</button>
    <UsuarioComponent :nome="nome" @nomeCurso="nome = $event"/>

  </div>
</template>

<script>
import UsuarioComponent from './components/Usuario.vue'
  export default{
    name: 'App',
    components:{
      UsuarioComponent
    },
    data(){
      return{
        nome: 'Fernanda Strebe'
      }
    },
    methods:{
      entrar(){
        this.nome = "Gabi";
      }
    }
  }
</script>


<style scoped>

</style>