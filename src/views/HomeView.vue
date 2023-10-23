<template>
    <v-row class="d-flex">
      <v-col cols="2">
        <LogoPielCanela />
      </v-col>
      <v-col>
        <TheWelcome />
      </v-col>
      <v-col cols="2">
        <IconosRedesSociales />
      </v-col>
    </v-row>
  </template>
  
  <script setup>
  import LogoPielCanela from '../components/LogoPielCanela.vue';
  import TheWelcome from '../components/TheWelcome.vue';
  import IconosRedesSociales from '../components/IconosRedesSociales.vue';
  </script>
  
  <style>
  .d-flex {
    display: flex;
    align-items: center; /* Alinea verticalmente en el centro */
  }
  </style>
  