<template>
    <div>
        <h1>Olá vue!</h1>
        <p> Meu Nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
        <Reutilizacao />
    </div>
</template>

<script>

    import MultiplosEventos from "./MultiplosEventos.vue";
    import Reutilizacao from "./Reutilizacao.vue";

    export default{
        name: "PrimeiroComponent",
        components:{
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return {
                nome: 'Cássio',
                profissao: 'Programador'
            }
        },
        
    }
</script>                       
