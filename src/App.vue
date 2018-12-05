<template>
  <div id="app">
    <div class="spieler1"></div>
    <div class= "spieler2"></div>
    <div class="spieler1"></div>
    <div class= "spieler2"></div>
    <div class="spieler1"></div>
    <div class= "spieler2"></div>
    <div class="spieler1"></div>
    <div class= "spieler2"></div>
    <div class="spieler1"></div>
  </div>
</template>

<script>
import Brett from './components/Brett.vue'

export default {
  name: 'app',
  components: {
    Brett
  }
}
</script>

<style>
#app {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-columns: 200px;
  margin: 0 auto;
  height: 600px;
  width: 600px;
  background: forestgreen;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.spieler1 {
  background: red;
  
}
</style>
