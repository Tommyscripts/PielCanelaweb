<template>
  <div  class="d-flex tamano">
    <v-col class="logo" cols="2">
      <LogoPielCanela />
    </v-col>
    <v-col cols="7" class="centered">
      <Identidad />
    </v-col>
    <v-col class="redes" cols="3">
      <IconosRedesSociales />
    </v-col>
  </div>

  <v-row class="mobile-view">
    <v-col cols="4">
      <LogoPielCanela />
    </v-col>

    <v-col cols="8">
      <Identidad />
      <IconosRedesSociales class="mobile-icons" />
    </v-col>
  </v-row>
</template>

<script setup>
import Identidad from '../components/Identidad.vue';
import LogoPielCanela from '../components/LogoPielCanela.vue';
import IconosRedesSociales from '../components/IconosRedesSociales.vue';
import IconosRedesSociales2 from '../components/IconosRedesSociales2.vue';
</script>

<style scoped>
.logo{
margin-bottom: 10vh;
}
.redes{
  margin-bottom: 10vh;
}
.tamano {
  height: 100%;
  width: 100%;
  background-color: black;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.mobile-view {
  display: none;
  /* Inicialmente ocultamos la vista de móvil */
}

.d-flex {
  display: flex;
}

.mobile-icons {
  flex-direction: row;
  margin-top: 1rem;
}

.desktop-icons {
  display: block;
}

.centered {
  margin: 0 auto;
}

.caja1 {
  position: relative;
}
</style>
