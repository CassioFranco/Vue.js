<template>
    <div>
        <img :src="avatar" :alt="descricao" width="200px">
        <Mudarimagem @mudarimagem="trocarimagem" />
    </div>
</template>

<script>
import Mudarimagem from './Mudarimagem.vue';

export default {
    name: 'Picture',
    components: {
        Mudarimagem
    },
    data() {
        return {
            avatar: '/public/img/ghost-custom.png',
            descricao: 'scream',
            isGhost: true
        }
    },
    methods: {
        trocarimagem() {
            if (this.isGhost) {
                this.avatar = '/public/img/vampire.png';
                this.descricao = 'vampire';
            } else {
                this.avatar = '/public/img/ghost-custom.png';
                this.descricao = 'scream';
            }
            this.isGhost = !this.isGhost;
            console.log("Imagem alternada");
        }
    }
}
</script>
