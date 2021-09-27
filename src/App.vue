<template>
  <div id="app">
    <Iniziale />
    <Main />
    <Finale />

  </div>
</template>

<script>
import Iniziale from './components/Iniziale.vue'
import Main from './components/Main.vue'
import Finale from './components/Finale.vue'


export default {
  name: 'App',
  components: {
    Iniziale,
    Main,
    Finale
  }
}
</script>

<style lang="scss">
@import "./components/style/variabili.scss";


#app {
  font-family: $headerfont, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: #2c3e50;
 
}
</style>
