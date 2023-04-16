<template>
  <firstComponent/>
  <lifeCycle/>
</template>

<script>
  import firstComponent from './components/firstComponent.vue'
  import lifeCycle from './components/lifeCycle.vue';

  export default {
      name: 'App',
      components: {
          firstComponent,
          lifeCycle
      }
  }

</script>