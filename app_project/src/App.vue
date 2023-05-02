<template>
  <Navbar :logo="logo_src" :alt="app_name"/>
  <router-view/>
  <ProjectFooter />
</template>


<script>
import Navbar from './components/Navbar.vue'
import ProjectFooter from './components/ProjectFooter.vue'

export default {
  components: {
    Navbar,
    ProjectFooter,
  },
  data() {
    return {
      logo_src: "./img/logo.png",
      app_name: "Make Your Burger"
    }
  },
}
</script>

<style>
  * {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  
</style>
