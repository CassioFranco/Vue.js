<template>
    <div>
        <h2>Meu Formulário:</h2>
        <form action="" @submit="enviarFormulario($event)">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <div>
                <submit />
            </div>
        </form>
        <p>Conteúdos</p>
        <p>Conteúdos</p>
        <p>Conteúdos</p>
    </div>
</template>
<script>
import submit from './form/submit.vue';
import inputText from './form/inputText.vue';
export default {
    name: 'Form',
    components: {
        inputText,
        submit
    },
    data() {
        return {
            name: "",
            email: ""
        }
    },

        
    methods: {
        enviarFormulario(e) {

            e.preventDefault();

            const name = this.name;
            const email = this.email;

            console.log("Formulário Enviado!");
            console.log("O nome é: " + name);
            console.log("O email é: " + email);

            // Ajax

            // inserir no banco os dados
        }
    }
}

</script>

<style scoped>
p {
    margin: 50px;
}
</style>
