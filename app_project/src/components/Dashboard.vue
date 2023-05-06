<template>
    <div id="burger-table">
        <div>
            <div id="burger-table-heading">
                <div class="order-id">#:</div>
                <div>Cliente: </div>
                <div>Pão:</div>
                <div>Carne:</div>
                <div>Opcionais:</div>
                <div>Ações</div>
            </div>
        </div>
        <div id="burger-table-rows">
            <div class="burger-table-row">
                <div class="order-number">1</div>
                <div>Nome Cliente</div>
                <div>Pão</div>
                <div>Carne</div>
                <div>
                    <ul>
                        <li>Salame</li>
                        <li>tomate</li>
                    </ul>
                </div>
            </div>
            <div>
                <select name="status" class="status">
                    <option value="">Selecione o Status do Hamburguer</option>
                </select>
                <button class="delete-btn">Cancelar</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Dashboard"
}

</script>

<style scoped>
</style>