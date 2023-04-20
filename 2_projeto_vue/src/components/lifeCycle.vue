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

        this.lifeCycle()
        },
        mounted() {
            setTimeout(() => {
            this.nome = 'Aleatorio'
        },  2000);
        this.lifeCycle()
        },
        methods: {
            lifeCycle() {
                console.log("executou")
            }
        }
    }

    
</script>
