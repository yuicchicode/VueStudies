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
            setTimeout(() => {
            this.nome = 'David'
        },  1000);
        },
        mounted() {
            setTimeout(() => {
            this.nome = 'Aleatorio'
        },  2000);
        },
    }

    
</script>
