<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p class="mover">Próximamente</p>
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
.mover{
  padding-left: 7em;
}
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
  font-size: 3vh;
  padding-right: 5em;
}

.playfair-display {
  font-family: 'Playfair Display', serif;
  font-size: 15vh;
  line-height: 1em;
  color:rgb(255, 255, 255);
}

.playfair-display .coming {
  position: relative;
}

.playfair-display .soon {
  position: relative;
  margin-left: -2.82em;
  top: 0.59em;
}

.bottom-text {
  margin-top: 4em;
  padding-left: 9em;
  /* Ajusta el margen superior según tus preferencias */
}

</style>
  