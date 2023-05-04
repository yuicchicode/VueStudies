<template>
    <div>
        <p>Componente de Mensagem</p>
        <div>
            <form id="burger-fomr">
                <div class="input-container">
                    <label for="nome">Nome do cliente</label>
                    <input type="text" id="nome" name="name" v-model="nome" placeholder="Digite o seu nome">
                </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: "BurgerForm"
}
</script>