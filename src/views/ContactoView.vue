!<template>
    <div class="d-flex tamano">
    <v-col cols="2">
      <LogoPielCanela />
    </v-col>
    <v-col cols="8">
        <Contacto />
    </v-col>
    <v-col cols="2">
      <IconosRedesSociales />
    </v-col>
  </div>
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
}

.d-flex {
  display: flex;
  justify-content: space-between;
  align-items: center;

}

.text-center {
  text-align: center;
}
</style>
