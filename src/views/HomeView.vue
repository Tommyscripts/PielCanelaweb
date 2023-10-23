<template>
  <v-container class="d-flex">
    <v-col cols="2">
      <LogoPielCanela />
    </v-col>
    <v-col cols="8">
      <TheWelcome />
    </v-col>
    <v-col cols="2">
      <IconosRedesSociales />
    </v-col>
  </v-container>
</template>

<script setup>
import LogoPielCanela from '../components/LogoPielCanela.vue';
import TheWelcome from '../components/TheWelcome.vue';
import IconosRedesSociales from '../components/IconosRedesSociales.vue';
</script>


<style>
.d-flex {
  display: flex;
  justify-content: space-between; /* Espacio uniforme entre los componentes */
  align-items: center; /* Alinea verticalmente en el centro */
}
.text-center {
  text-align: center; /* Alineación horizontal en el centro */
}
</style>
