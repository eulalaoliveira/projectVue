<template>
    <div>
        <h2>Essa é a descrição da pessoa: {{ nome }} </h2>
        <Info :email="email" :esta_trabalhando=true />
        <Form />
    </div>
</template>
<script>
    import Info from "./Info.vue"
    import Form from "./Form.vue"

    export default {
        name: 'Pessoa',
        components: {
            Info,
            Form
        },
        data() {
            return {
                nome: "Matheus",
                email: "matheus2@email.com"
            }
        }
    }
</script>
