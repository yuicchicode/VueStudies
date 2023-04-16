<template>
    <div>
        <h1>Opa Vue!</h1>
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    </div>
</template>

<script>

    export default {
        name: 'firstComponent',
        data() {
            return {
                nome: "David",
                profissao: "Desenvolvedor"
            }
        },
    }


</script>