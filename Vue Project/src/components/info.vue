<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else ></p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
        <div>
            <button @click="showEmail">{{ textobotao }}</button>
        </div>
        <p v-show='mostrar_email'>Mande uma mensagem para: {{ email }}</p>
        <p class="teste">Para acessar meu portfólio basta <a v-bind:href="meu_link" target="_blank">clicar aqui.</a></p>
        <Picture />
    </div>
</template>
<script lang="ts">

import Picture from "./Picture.vue"

export default {
    name: 'info',
    components:{
        Picture
    },
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: false,
            email: 'cassio-franco@hotmail.com',
            meu_link: 'https://google.com',
            textobotao: 'Mostrar e-mail'

        }
    },
    methods:{
        showEmail(){
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email){
                this.textobotao = 'Mostrar e-mail'
            }else{
                this.textobotao = 'Esconder e-mail'
            }
        }
    }
}
</script>

<style>
    .paragrafo-pai{
        color: red;
    }
</style>