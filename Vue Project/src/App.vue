<template>
  <div>
    <primeiro-component />
    <p>O dado de app é: {{ testando }}</p>
    <life-cycle />
    <Pessoa />
  </div>
  
</template>

<script>
  import PrimeiroComponent from './components/PrimeiroComponent.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';

  export default {
    name:'App',
    components: {
      PrimeiroComponent,
      LifeCycle,
      Pessoa
    },
    data() {
      return {
        testando: 'Teste'
      }
    },
    
  }
</script>