<template>
  <div class="d-flex tamano">
    <v-col cols="12" md="2">
      <LogoPielCanela class="logo-left" />
    </v-col>
    <v-col cols="12" md="8">
      <Contacto />
    </v-col>
    <v-col cols="12" md="2">
      <IconosRedesSociales />
    </v-col>
  </div>

  <v-row class="mobile-view">
      <v-col cols="4">
        <LogoPielCanela />
      </v-col>

      <v-col cols="8">
        <Contacto />
        <IconosRedesSociales class="mobile-icons" />
      </v-col>
    </v-row>
</template>

<script setup>
import Contacto from '../components/Contacto.vue';
import LogoPielCanela from '../components/LogoPielCanela.vue';
import IconosRedesSociales from '../components/IconosRedesSociales.vue';
</script>

<style scoped>
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

.caja1 {
  position: relative;
}


</style>
