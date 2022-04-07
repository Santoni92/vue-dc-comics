<template>
  <div id="app">
    <Header :links="menu"/>
    <Main :posters="locandine"/>
    <Contatti :contacts="contatti"/>
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
// data
import locandine from '@/assets/dc-comics'; //importo la struttura dati presente nel file .json
import contatti from '@/assets/contatti'

export default {
  name: "App",
  data(){
    return {
      menu:['CHARACTERS','COMICS','MOVIES','TV','GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS','SHOP'],  //faccio il return della struttura dati così da poterne fare il rendering nel componente tramite la props
      locandine,
      //contatti: ['DIGITAL COMICS','DC MERCHANDISING','SUBSCRIPTION','COMIC SHOP LOCATOR','DC POWER VISA']
      contatti
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
