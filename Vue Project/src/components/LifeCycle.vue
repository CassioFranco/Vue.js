<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name: 'LyfeCycle',
        data() {
            return {
                nome: 'Marya'
            }
        },
        created() {
            setTimeout (() => {
                this.nome = 'Pedro'
            }, 1000)
        },
        mounted() {
            setTimeout (() => {
                this.nome = 'Cássio'
            }, 2000);
        }
    }
</script>
