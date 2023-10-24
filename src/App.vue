<template>
  <div class="app">
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
import Navbar from './components/nav-bar.vue';
import TheWelcome from './views/HomeView.vue';
import Identidad from './views/IdentidadView.vue';
import Contacto from './views/ContactoView.vue';
export default {
  components: {
    Navbar,
    TheWelcome,
    Identidad,
    Contacto
},
  data() {
    return {
      currentTab: 'tab1',
    };
  },
  methods: {
    changeTab(tab) {
      this.currentTab = tab;
    },
  },
};
</script>

<style scoped>
.app {
  height: 99vh; /* Altura de la ventana del navegador */
  width: 99vw; /* Ancho de la ventana del navegador */
  background-color: black;
  margin: 0; /* Elimina márgenes predeterminados */
  padding: 0; /* Elimina relleno predeterminado */
  overflow: hidden; /* Evita barras de desplazamiento */
}

.content {
  height: 100%; /* Asegura que el contenido ocupe la pantalla completa */
  width: 100%;
}
</style>
