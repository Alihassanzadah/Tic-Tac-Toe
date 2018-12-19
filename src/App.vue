<template>
  <div id="app">
    <h1> TicTacToe</h1>
    <div id= "detail">
      <h2>Turn player {{spieler}} </h2>
    <grid v-on:playerClickt ="updatedSpieler($event)"></grid>
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
      spieler: ''
    }
  },
  methods: {
     updatedSpieler : function(updatedSpieler) {
      this.spieler = updatedSpieler;
    }
  }
   
}
</script>

<style scoped>
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
h2 {
  color: dimgray;
  padding: 15px;
  margin: 0 auto;
}
</style>
