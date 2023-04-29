<template>
    <div>
        <button @click="$emit('mudarImagem')">Trocar Foto</button>
    </div>
</template>

<script>
export default {
    name: 'MudarImagem',
    emits: ['mudarImagem']
}
</script>