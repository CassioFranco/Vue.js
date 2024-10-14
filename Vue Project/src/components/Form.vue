<template>
    <div>
        <h2>Meu Formulário:</h2>
    <form action="">
        <div>
            <inputText />
        </div>
        <div>
            <inputText />
        </div>
        <div>
            <submit/>
        </div>
    </form>
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
        }
    }

</script>
