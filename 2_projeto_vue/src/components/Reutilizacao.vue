<template>
    <div>
        <button @click="ativar">Clique aqui</button>
        <span v-show="ativou">Ativado!</span>
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue'
    import Reutilizacao from './Reutilizacao.vue'

    export default{
        name: 'Reutilizacao',
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return {
                ativou: false
            }
        },
        methods: {
            ativar() {
                this.ativou = !this.ativou
            }
        },
    }
</script>