<template>
  <div class="app">
    <Navbar @tab-change="changeTab" />
    <div class="content">
      <div v-if="currentTab === 'tab1'">
        <TheWelcome />
      </div>
      <div v-if="currentTab === 'tab2'">Contenido de la Pestaña 2</div>
      <div v-if="currentTab === 'tab3'">Contenido de la Pestaña 3</div>
    </div>
  </div>
</template>

<script>
import Navbar from './components/nav-bar.vue';
import TheWelcome from './views/HomeView.vue';
export default {
  components: {
    Navbar,
    TheWelcome
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
  width: 100vh;
  background-color: black;
}

.content {
  padding: 20px;
  height: 100%;
  width: 100%;
}
</style>
