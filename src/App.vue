<template>
  <div id="app">
    <MeteoDetails v-bind="meteo_data" />
  </div>
</template>

<script>
import MeteoDetails from './components/MeteoDetails.vue'

export default {
  name: 'App',
  components: {
    MeteoDetails
  },
  data: () => ({
    meteo_data: {
      ville:"Paris",
      description:"Nuageux",
      temperature: 25,
      humidity: 50,
      pressure: 1021,
      wind_speed: 14,
      icon_url: ""
    }
  })
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
