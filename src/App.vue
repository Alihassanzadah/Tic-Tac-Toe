<template>
  <div id="app">
    <h1> TicTacToe</h1>
    <div id= "detail">
      <h2>Turn {{spieler1 & 2}}</h2>
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
      spieler1: function(currentPlayer = 1) {
        this.spieler1= 'spieler1'
      },
      spieler2: function(currentPlayer = 1){
        this.spieler2= 'spieler2'
      }
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
#detail {
  height: 650px;
  width: 600px;
  background: orange;
  margin: 0 auto;
}
</style>
