<template>
  <div id="app">
    <Chartbox />
  </div>
</template>

<script>
import Chartbox from './components/Chartbox.vue'

export default {
  name: 'app',
  components: {
    Chartbox
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
