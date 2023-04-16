<template>
  <div>
    <firstComponent/>
    <lifeCycle/>
    <person/>
  </div>  
</template>

<script>
  import firstComponent from './components/firstComponent.vue'
  import lifeCycle from './components/lifeCycle.vue';
  import person from './components/person.vue';

  export default {
      name: 'App',
      components: {
          firstComponent,
          lifeCycle,
          person
      }
  }

</script>