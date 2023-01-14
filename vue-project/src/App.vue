<template>
  <div>
    <Header :esta_logado="true" />
    <PrimeiroComponente />
    <p>O dado de app é {{ testando }}</p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
  import PrimeiroComponente from "../src/components/PrimeiroComponente.vue" 
  import LifeCycle from "../src/components/LifeCycle.vue"
  import Pessoa from './components/Pessoa.vue'
  import Header from "./components/Header.vue"

  export default {
    name: "app",
    components: {
      Header,
      PrimeiroComponente,
      LifeCycle,
      Pessoa
    },
    data() {
        return {
            testando: "Teste"
        }
    }
  }
</script>