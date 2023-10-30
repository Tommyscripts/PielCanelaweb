<template>
  <!-- Vista de PC -->
  <div class="d-flex tamano">
    <v-col cols="2" md="2">
      <LogoPielCanela />
    </v-col>
    <v-col cols="8" md="4">
      <div class="caja1">
        <Contacto />
      </div>
    </v-col>
    <v-col cols="2" md="2">
      <IconosRedesSociales />
    </v-col>
  </div>

  <!-- Vista de móvil -->
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
