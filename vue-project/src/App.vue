<template>
  <div>
    <PrimeiroComponente />
    <p>O dado de app é {{ testando }}</p>
    <LifeCycle />
  </div>
</template>

<script>
  import PrimeiroComponente from "../src/components/PrimeiroComponente.vue" 
  import LifeCycle from "../src/components/LifeCycle.vue"

  export default {
    name: "app",
    components: {
      PrimeiroComponente,
      LifeCycle
    },
    data() {
        return {
            testando: "Teste"
        }
    }
  }
</script>