<template>
  <v-main>
    <div class="app">
      <Navbar @tab-change="changeTab" />
      <img src="./assets/slidemouse.gif" alt="GIF" class="global-gif" />
      <div class="content">
        <div v-if="currentTab === 'tab1'" :key="'tab1'">
          <TheWelcome />
        </div>
        <div v-if="currentTab === 'tab2'" :key="'tab2'">
          <Identidad />
        </div>
        <div v-if="currentTab === 'tab3'" :key="'tab3'">
          <Contacto />
        </div>
      </div>
    </div>
  </v-main>
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
  height: 100vh;
  width: 100vw;
  background-color: black;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

.content {
  height: 100%;
  width: 100%;
}

.global-gif {
  position: fixed;
  bottom: 2.8rem; /* Ajusta la distancia desde la parte inferior */
  left: 51%;
  transform: translateX(-50%);
  width: 4vh; /* Ajusta el tamaño del GIF según tus preferencias */
}
</style>
