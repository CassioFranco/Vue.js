<template>
    <div>
        <button @click="$emit('mudarimagem')">Trocar imagem de perfil</button>
    </div>
</template>

<script>
    export default {
        name: "Mudarimagem",
        emits: ['mudarimagem']
    }
</script>