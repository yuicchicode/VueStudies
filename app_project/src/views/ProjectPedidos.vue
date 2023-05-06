<template>
    <Banner />
    <div class="main-container">
        <h1>Gerenciar pedidos:</h1>
        <Dashboard />
    </div>
</template>

<script>
import Dashboard from '@/components/Dashboard.vue';
import Banner from '@/components/Banner.vue'

export default {
    name: "Pedidos",
    components: {
    Dashboard,
    Banner
}
}
</script>