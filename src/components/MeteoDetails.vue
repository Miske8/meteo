<template>
  <div class="meteo-wrapper">
    <div class="header">
      <div>
        <h1>{{ ville }}</h1>
        <h2>{{ description }}</h2>
      </div>
      <img id="meteo-icon" :src="icon_url" />
    </div>
    <div class="content">
      <div class="item">Temperature:{{temperature}} °C</div>
      <div class="item">Humidité:{{humidity}} %</div>
      <div class="item">Pression: {{pressure}} hPa</div>
      <div class="item">Vent:{{wind_speed}} m/s</div>
    </div>
  </div>
    </template>

<script>
export default {
  name: 'MeteoDetails',
  props: {
    ville: {
      type: String,
      required: false
    },
    description: {
      type: String,
      required: true
    },
    temperature: {
      type: Number ,
      required: true
    },
    humidity: {
      type: Number ,
      required: true
    },
    pressure: {
      type: Number ,
      required: true
    },
    wind_speed: {
      type: Number ,
      required: true
    },
    icon_url:""
  }
}
</script>

<style scoped>
.meteo-wrapper {
  background-color: grey;
}
</style>
