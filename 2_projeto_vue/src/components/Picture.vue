<template>
    <div>
        <img :src="avatar" alt="descricao">
        <MudarImagem @mudar-imagem="trocarImagem"/>
    </div>
</template>

<script>
    import MudarImagem from './MudarImagem.vue';

    export default {
        name: 'Pìcture',
        components: {
            MudarImagem
        },
        data() {
            return {
                avatar: "/img/avatar.png",
                descricao: "David Benhur"
            }
        },
        methods: {
            trocarImagem() {
                this.avatar = "/img/avatar2.png"
            }
        }
    }
</script>