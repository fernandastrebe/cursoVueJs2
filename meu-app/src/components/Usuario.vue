<template>
    <div id="usuario">
        <h2>Olá {{nome}}</h2>
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
    }
}
</script>

<style scoped>
    
</style>