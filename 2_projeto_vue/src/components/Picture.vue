<template>
    <div>
        <img :src="avatar" alt="descricao">
    </div>
</template>

<script>
    export default {
        name: 'Pìcture',
        data() {
            return {
                avatar: "/img/avatar.png",
                descricao: "David Benhur"
            }
        },
    }
</script>