<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
    export default{
        name:'Picture',
        data(){
            return{
                avatar: '/public/img/ghost-custom.png',
                descricao: 'banana'
            }
        }
    }
</script>
