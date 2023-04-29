<template>

    <div>
        <p>{{ compEmail }} - {{ email }}</p>
        <p v-if="esta_trabalhando"> Estou trabalhando no momento. </p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li v-for="(techology, index) in backend_technologies" v-bind:key="index">{{ techology }}</li>
        </ul>
        <p>Tecnologias para front-end</p>
        <ul>
            <li v-for="technology in frontend_technologies" :key="technology.id">{{ technology.language }}</li>
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
        name: 'info',
        components: { 
        Picture 
    },
    props: {
        email: String,
        esta_trabalhando: Boolean
    },
    data() {
        return {
            mostrar_email: false,
            meu_link: 'https://google.com',
            buttonText: 'Mostrar E-mail',
            backend_technologies: [
                'JavaScript',
                'C#',
                'Python',
                'Nodejs',
            ],
            frontend_technologies:[
                {id: 1, language: 'HTML'},
                {id: 2, language: 'CSS'},
                {id: 3, language: 'Vue'},
            ],
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