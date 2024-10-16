<template>
    <div>
        <button @click="primeiro($event), segundo($event), terceiro($event)">Ativar Múltiplos Eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
export default {
    name: 'MultiplosEventos',
    data() {
        return {
            multiplos_eventos: ""
        }
    },
    methods: {
        primeiro(e) {
            this.multiplos_eventos = "Primeiro evento ativado!"
        },
        segundo(e) {
            setTimeout(() => {
                this.multiplos_eventos = "Segundo evento ativado!"
            }, 500)
        },
        terceiro(e) {
            setTimeout(() => {
                this.multiplos_eventos = ""
            }, 1000)
        }

    },
} 
</script>

<style scoped>
div {
    margin: 100px;
}
</style>
