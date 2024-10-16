<template>
    <div>
        <h1>Olá vue!</h1>
        <p> Meu Nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>

    import MultiplosEventos from "./MultiplosEventos.vue"

    export default{
        name: "PrimeiroComponent",
        components:{
            MultiplosEventos
        },
        data() {
            return {
                nome: 'Cássio',
                profissao: 'Programador'
            }
        },
        
    }
</script>
