<template>
    <div>
        <h1>Opa Vue!</h1>
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos/>
        <reutilizacao/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import Reutilizacao from './Reutilizacao.vue'

    export default {
        name: 'firstComponent',
        components: {
            MultiplosEventos,
                Reutilizacao
        },
        data() {
            return {
                nome: "David",
                profissao: "Desenvolvedor"
            }
        },
    }


</script>