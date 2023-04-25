<template>

    <div>
        <p v-if="esta_trabalhando"> Estou trabalhando no momento. </p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>JavaScript</li>
            <li>HTML e CSS</li>
            <li>Vue.js</li>
            <li>Node.js</li>
        </ul>
        <div>
            <button @click="showEmail"> {{buttonText}} </button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p class="teste">Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
    <Picture />
    </div>

</template>


<script>
import Picture from './Picture.vue'

    export default {
    components: { Picture },
    name: 'info' ,
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "teste@gmail.com",
            meu_link: 'https://google.com',
            buttonText: 'Mostrar E-mail'
            }
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email){
                    this.buttonText = 'mostrar e-mail'
                } else {
                    this.buttonText = "ocultar e-mail"
                }
            }
        },        
    }

</script>

<style>
    .paragrafo-pai{
        color: red;
    }
</style>