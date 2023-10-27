<template>
  <div class="app" @scroll="handleScroll">
    <Navbar @tab-change="changeTab" />
    <div class="content">
      <div v-if="currentTab === 'tab1'">
        <TheWelcome />
      </div>
      <div v-if="currentTab === 'tab2'">
        <Identidad />
      </div>
      <div v-if="currentTab === 'tab3'">
        <Contacto />
      </div>
    </div>
  </div>
</template>

<script>
import TheWelcome from './HomeView.vue';
import Navbar from '@/components/Navbar.vue';
import Identidad from './IdentidadView.vue';
import Contacto from './ContactoView.vue'

export default {
  components: {
    Navbar,
    TheWelcome,
  },
  data() {
    return {
      currentTab: 'tab1', // Inicialmente, muestra el contenido de 'TheWelcome'
    };
  },
  methods: {
    changeTab(tab) {
      this.currentTab = tab;
    },
    handleScroll(event) {
      if (event.deltaY > 0) {
        // Scroll hacia abajo, cambia a la siguiente pestaña
        this.changeTab('tab2'); // Cambia a la pestaña siguiente
      } else {
        // Scroll hacia arriba, cambia a la pestaña anterior
        this.changeTab('tab1'); // Cambia a la pestaña anterior
      }
    },
  },
};
</script>

<style scoped>
.app {
  height: 100vh;
  /* Altura de la ventana del navegador */
  width: 100%;
  background-color: black;
  overflow-y: scroll; /* Habilita el scroll vertical en la vista */
}

.content {
  padding: 20px;
  height: 100%;
  /* Asegura que el contenido ocupe la pantalla completa */
  width: 100%;
}</style>
