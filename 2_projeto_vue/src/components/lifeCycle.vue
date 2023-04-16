<template>
    <div>
        <h1>Meu nome é: {{ nome }}</h1>
    </div>
</template>

<script>

    export default {
        name: 'lyfeCycle',
        data() {
            return {
                nome: 'Testes'
            }
        },
        created() {
            this.nome = 'David'
        },
    }

</script>
