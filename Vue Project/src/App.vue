<style>
body {
  background-color: #333;
  color: #FFF;
}

a {
  color: red;
}

.teste {
  background-color: black;
}
</style>


<template>
  <div>
    <Header />
    <primeiro-component />
    <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
    <life-cycle />
    <Pessoa />
  </div>

</template>

<script>
import Header from './components/Header.vue';
import PrimeiroComponent from './components/PrimeiroComponent.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

export default {
  name: 'App',
  components: {
    Header,
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
