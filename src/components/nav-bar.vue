<template>
  <div class="navbar">
    <div class="menu-icon" @click="changeTab('tab1')"></div>
    <div class="menu-icon" @click="changeTab('tab2')"></div>
    <div class="menu-icon" @click="changeTab('tab3')"></div>
  </div>
</template>


<script>

export default {
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
  /* Color de fondo */
  padding: 10px;
  /* Espacio alrededor de los puntos */
}

.menu-icon {
  width: 10px;
  /* Ancho del punto */
  height: 10px;
  /* Alto del punto */
  background-color: #fff;
  /* Color del punto */
  border-radius: 50%;
  /* Hace que el punto sea circular */
  margin: 0 10px;
  /* Espacio entre los puntos */
  cursor: pointer;
  /* Cambia el cursor al pasar por encima */
}</style>
