<template>
    <div id ="game" class= "grid">
    <div v-for="(color, index) in backgroundColors" v-bind:key="index" v-on:click.once="playerClickt(index)" :class="['spieler1', 'spieler2', color]" ></div>  
  </div>
</template>

<script>
export default {
  name: 'grid',
  data() {
    return {
      backgroundColors: [
        'transparent',
        'transparent',
        'transparent',
        'transparent',
        'transparent',
        'transparent',
        'transparent',
        'transparent',
        'transparent'
      ],
      currentPlayer: 1,
    }
  },
  methods: {
    playerClickt(field){
      
      if(this.currentPlayer == 1){
        Vue.set(this.backgroundColors, field, 'green')
        this.currentPlayer = 2,
        this.$emit('playerClickt','red')
      }else{
        Vue.set(this.backgroundColors, field, 'red')
        this.currentPlayer = 1
        this.$emit('playerClickt', 'green')
        
        
      }
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#game {
  background-color: #844346
}
.grid {
  background: saddlebrown;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-columns: 200px;
  margin: 0 auto;
  height: 600px;
  width: 600px;
  border: 2px solid white;
}
.spieler1 {

 border: 1px solid white;
}
.spieler2 {
   border: 1px solid white;

}

.green{
  background-color: green;
}

.red{
  background-color: red;
}
</style>
