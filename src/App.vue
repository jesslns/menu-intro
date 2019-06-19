<template>
  <div id="app">
    <navigation></navigation>
    <img src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<script>
// import nav bar component to all the pages
import Navigation from './components/Nav'

export default {
  name: 'App',
  components: {
    'navigation': Navigation
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
