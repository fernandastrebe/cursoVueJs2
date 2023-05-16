<template>
    <div id="usuario">
        <h2>Olá {{nome}}</h2>
        <button @click="curso">NOME CURSO</button>
    </div>
</template>

<script>
export default {
    name: 'UsuarioComponent',
    props: {
        nome:{
            type: String,
            required: true
        }
    },
    methods:{
        curso(){
            this.nome = 'Aprendendo português';
            this.$emit('nomeCurso', this.nome);
        }
    }
}
</script>

<style scoped>
    
</style>