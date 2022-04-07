<template>
  <div id="app">
    <Header :links="menu"/>
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
  data(){
    return {
      menu:['CHARACTERS','COMICS','MOVIES','TV','GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS','SHOP']
      }
  },
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
