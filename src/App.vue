/* Esercizio di oggi: Vue DC Comics nome repo: vue-dc-comics Descrizione: Create
un nuovo progetto utilizzando Vue CLI e definite i componenti necessari per
strutturare il layout come da screenshot allegato. Quando la struttura a
macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del
componente. Per oggi diamo priorità alla struttura: quando è tutto bello solido,
passiamo al Sass! Bonus: Creare un componente aggiuntivo per gestire la fascia
azzurra con le icone. Da ricordare: creare il nuovo progetto, modalità manuale,
installando sass (guardate la parte finale delle slide di venerdì) quando
sviluppiamo lanciamo e teniamo aperto il comando npm run serve prima del push,
CTRL + C per chiudere il processo di npm run serve, e poi npm run build La prima
volta sarà necessario eliminare dist/ dal .gitignore. Qui la repo di oggi:
https://github.com/ott-fogliata/vue-molisana In allegato tutto il materiale per
l’esercizio. */

<template>
  <div id="app">
    <Header />
    <Main />
    <MainSectionBlue />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import MainSectionBlue from './components/MainSectionBlue.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    MainSectionBlue,
    Footer,
  },
}
</script>

<style lang="scss">
@import './style/app.scss';

MainSectionBlue {
  position: relative;
  z-index: 20;
}

Footer {
  position: relative;
  z-index: 30;
}
</style>
