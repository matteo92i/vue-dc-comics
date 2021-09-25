<template>
  <div id="app">
    <Header />
    <Central />
    <Footer />

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Central from './components/Central.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Central,
    Footer
  }
}
</script>

<style lang="scss">
@import "./components/style/variabili.scss";


#app {
  font-family: $headerfont, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
