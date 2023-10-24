<template>
  <div class="navbar">
    <div
      class="menu-icon"
      v-for="tab in tabs"
      :key="tab"
      @click="changeTab(tab)"
      :class="{ 'active': currentTab === tab }"
      tabindex="0" 
    ></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tabs: ['tab1', 'tab2', 'tab3'], // Agrega aquí todas tus pestañas
    };
  },
  methods: {
    changeTab(tab) {
      this.$emit('tab-change', tab);
    },
  },
};
</script>

<style>
.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #000;
  padding: 10px;
}

.menu-icon {
  width: 10px;
  height: 10px;
  background-color: #827d7d; /* Establece el color gris predeterminado */
  border-radius: 50%;
  margin: 0 10px;
  cursor: pointer;
  transition: background-color 0.3s; /* Agrega una transición para suavizar el cambio de color */
}

.menu-icon:focus {
  background-color: #fff; /* Establece el color blanco para el enfoque */
}

.active {
  background-color: #fff; /* Establece el color blanco para la pestaña activa */
}
</style>
