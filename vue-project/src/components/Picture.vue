<template>
    <img :src="avatar" :alt="descricao">
    <Reutilizacao />
</template>
<script>
import Reutilizacao from "./Reutilizacao.vue";

    export default {
        name: "Picture",
        data() {
            return {
                avatar: "/img/avatar.png",
                descricao: "Matheus Battisti"
            }
        },
        components: {
            Reutilizacao,
        }
    }
</script>
