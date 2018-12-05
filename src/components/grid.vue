<template>
    <div class= "grid">
    <div v-on:click= "red" class="spieler1"></div>
    <div v-on:click= "green" class= "spieler2"></div>
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
export default {
  name: 'grid',
  data() {
    return {
      
    }

  


  },
    methods: {
      red: function () {
        
      }
      
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.grid {
  background: saddlebrown;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-columns: 200px;
  margin: 0 auto;
  height: 600px;
  width: 600px;
}
</style>
