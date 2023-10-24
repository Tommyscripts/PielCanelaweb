<template>
  <div class="app">
    <Navbar @tab-change="changeTab" />
    <div class="content">
      <div v-if="currentTab === 'tab1'">
        <TheWelcome />
      </div>
      <div v-if="currentTab === 'tab2'"> <Identidad/> </div>
      <div v-if="currentTab === 'tab3'">Contenido de la Pestaña 3</div>
    </div>
  </div>
</template>

<script>
import TheWelcome from './HomeView.vue';
import Navbar from '@/components/Navbar.vue';
import Identidad from'./IdentidadView.vue';

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
  },
};
</script>

<style scoped>
.app {
  height: 100vh;
  /* Altura de la ventana del navegador */
  width: 100%;
  background-color: black;
}

.content {
  padding: 20px;
  height: 100%;
  /* Asegura que el contenido ocupe la pantalla completa */
  width: 100%;
}
</style>