<template>
    <div>
        <h1>Opa Vue!</h1>
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'

    export default {
        name: 'firstComponent',
        components: {
            MultiplosEventos
        },
        data() {
            return {
                nome: "David",
                profissao: "Desenvolvedor"
            }
        },
    }


</script>