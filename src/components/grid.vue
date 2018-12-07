<template>
    <div id ="game" class= "grid">
    <div v-on:click= "background1 = 'red'" v-bind:style="{ backgroundColor: background1 }" class="spieler1"></div>
    <div v-on:click= "background2 = 'green'" v-bind:style="{ backgroundColor: background2 }" class="spieler2"></div>
   <div v-on:click= "background3 = 'red'" v-bind:style="{ backgroundColor: background3 }" class="spieler1"></div>
    <div v-on:click= "background4 = 'green'" v-bind:style="{ backgroundColor: background4 }" class="spieler2"></div>
    <div v-on:click= "background5 = 'red'" v-bind:style="{ backgroundColor: background5 }" class="spieler1"></div>
    <div v-on:click= "background6 = 'green'" v-bind:style="{ backgroundColor: background6 }" class="spieler2"></div>
    <div v-on:click= "background7 = 'red'" v-bind:style="{ backgroundColor: background7 }" class="spieler1"></div>
    <div v-on:click= "background8 = 'green'" v-bind:style="{ backgroundColor: background8 }" class="spieler2"></div>
    <div v-on:click= "background9 = 'red'" v-bind:style="{ backgroundColor: background9 }" class="spieler1"></div>
  </div>
</template>

<script>
export default {
  name: 'grid',
  data() {
    return {
    background1: String,
    background2: String,
    background3: String,
    background4: String,
    background5: String,
    background6: String,
    background7: String,
    background8: String,
    background9: String,
      }
  },
  methods: {
  
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
</style>
