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
  #nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
</style>
