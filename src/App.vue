<template>
  <div id="app">
    <Header/>
    <Main/>
    <Contatti/>
    <Informazioni/>
    <Footer/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Contatti from './components/Contatti.vue'
import Informazioni from './components/Informazioni.vue'
import Footer from './components/Footer.vue'

export default {
  name: "App",
  components: {
    Header,
    Main,
    Contatti,
    Informazioni,
    Footer
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display:flex;
  flex-direction: column;
}
</style>
