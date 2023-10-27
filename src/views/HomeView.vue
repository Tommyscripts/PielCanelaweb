<template>
  <div class="d-flex tamano">
    <v-col cols="2">
      <LogoPielCanela />
    </v-col>
    <v-col cols="8">
      <div class="caja1">
        <TheWelcome />
        <div class="mobile-icons">
          <IconosRedesSociales />
        </div>
      </div>
    </v-col>
    <v-col cols="2" class="desktop-icons">
      <IconosRedesSociales />
    </v-col>
  </div>
</template>

<script setup>
import LogoPielCanela from '../components/LogoPielCanela.vue';
import TheWelcome from '../components/TheWelcome.vue';
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

.d-flex {
  display: flex;
}

.mobile-icons {
  display: none;
}

.desktop-icons {
  display: block;
}

.caja1 {
  position: relative;
}

/* Media query para pantallas con un ancho máximo de 900px (ajustado para dispositivos similares al iPhone SE) */
@media (max-width: 900px) {
  .mobile-icons {
    display: flex;
    flex-direction: row; /* Mostramos los iconos horizontalmente en la vista móvil */
    justify-content: center; /* Centramos los iconos horizontalmente en la vista móvil */
  }
  .desktop-icons {
    display: none;
  }
  .caja1 {
    position: relative; /* Aseguramos que 'caja1' siga siendo 'relative' */
  }
}
</style>
