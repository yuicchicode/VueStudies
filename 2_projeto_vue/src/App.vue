<template>
  <div>
    <Header />
    <firstComponent/>
    <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
    <lifeCycle/>
    <person/>
  </div>  
</template>

<script>
  import Header from './components/Header.vue'
  import firstComponent from './components/firstComponent.vue'
  import lifeCycle from './components/lifeCycle.vue';
  import person from './components/person.vue';

  export default {
      name: 'App',
      components: {
          Header,
          firstComponent,
          lifeCycle,
          person
      },
      data() {
        return {
          testando: "teste"
        }
      },
  }

</script>

<style>
  body{
    background-color: #000;
    color: rgba(124, 116, 116);
  }

  a{
    color: red;
  }

  .teste{
    background-color: aliceblue;
  }
</style>