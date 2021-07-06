<template>
  <div id="app">
    <MeteoDetails />
  </div>
</template>

<script>
import MeteoDetails from './components/MeteoDetails.vue'

export default {
  name: 'App',
  components: {
    MeteoDetails
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
  margin-top: 60px;
}
</style>
