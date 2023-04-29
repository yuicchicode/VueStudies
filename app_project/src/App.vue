<template>
  <Navbar />
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
  }
}
</script>

<style>

</style>
