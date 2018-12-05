<template>
  <div id="app">
    <h1> TicTacToe</h1>
    <div id= "detail">
      <h2>Turn </h2>
    <grid></grid>
  </div>
    </div>
   
</template>

<script>
import grid from './components/grid.vue'

export default {
  components: {
    grid
  },
  data() {
    return {

    }

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
.spieler1 {
  background: red;
  
}
</style>
