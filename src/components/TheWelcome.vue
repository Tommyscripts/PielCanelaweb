<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p>Próximamente</p>
      <v-divider></v-divider>
      <div class="playfair-display">
        <span class="coming">Coming</span>
        <span class="soon">Soon</span>
      </div>
      <v-divider></v-divider>
      <div class="bottom-text">
        Pronto podréis explorar una experiencia completamente nueva y mejorada.
        <br>
        ¡Mantente atento para descubrir nuestras novedades!
      </div>
    </div>
  </div>
</template>
  
<script>
export default {
};
</script>
  
<style scoped>
.full-width {
  width: 100%;
}

.centered-text {
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  font-family: 'Raleway', sans-serif;
}

.playfair-display {
  font-family: 'Playfair Display', serif;
  font-size: 10vh;
  line-height: 1em;
}

.playfair-display .coming {
  position: relative;
  margin-right: -0.1em;
}

.playfair-display .soon {
  position: relative;
  margin-left: -2.4em;
  top: 0.56em;
}

.bottom-text {
  margin-top: 5em;
  /* Ajusta el margen superior según tus preferencias */
}
</style>
  