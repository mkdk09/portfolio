<template>
  <div id="app">
    <navbar />
    <profile />
    <skill />
    <works />
  </div>
</template>

<script>
import navbar from './components/Navbar.vue'
import profile from './views/profile.vue'
import skill from './views/skill.vue'
import works from './views/works.vue'

export default {
  name: 'App',
  components: {
    profile,
    skill,
    works,
    navbar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 40px;
}

#profile {
  padding-top: 40px;
}

#skill {
  padding-top: 40px;
}

#works {
  padding-top: 40px;
}
</style>
