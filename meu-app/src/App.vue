<template>
  <div id="app">
    <h1>Bem-vindo ao meu primeiro projeto!</h1>
    <UsuarioComponent/>
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
        nome: 'Fernanda'
      }
    },
    methods:{

    }
  }
</script>

<style scoped>

</style>