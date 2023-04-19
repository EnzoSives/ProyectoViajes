<template>
  <div id="app">
    <navbar />
    <background-image :image-url="backgroundImageUrl">
      <comparar-vuelos/>
    </background-image>
    <titulo-pag title="Ultimos vuelos" />
    <cards-vuelos />
    <br>
    <titulo-pag title="Noticias" />
    <novedades-vuelos />
    <br>
    <Footer />


    <router-view />
  </div>
</template>

<script>
import Navbar from './components/NavBar.vue';
import BackgroundImage from './components/BackgroundImage.vue';
import CompararVuelos from './components/CompararVuelos.vue';
import TituloPag from './components/TituloPag.vue';
import CardsVuelos from './components/CardsVuelos.vue';
import NovedadesVuelos from './components/NovedadesVuelos.vue'
import Footer from './components/FooterPage.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    BackgroundImage,
    CompararVuelos,
    TituloPag,
    CardsVuelos,
    NovedadesVuelos,
    Footer
  },
  data() {
    return {
      backgroundImageUrl: 'https://i0.wp.com/sinmordaza.com/wp-content/uploads/2021/10/vuelos-baratos-paginas-b.jpg?fit=1140%2C854&ssl=1',
    };
  },
  
};
</script>

<style>

</style>
