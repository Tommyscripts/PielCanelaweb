<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p class="mover" style="font-style: italic;">Próximamente</p>
      <br>
      <br>
      <div class="playfair-display">
        <span class="coming" style="font-style: italic;">Coming</span>
        <span class="soon" style="font-style: italic;">Soon</span>
      </div>
      <br>
      <br>
      <div class="bottom-text" style="font-style: italic;">
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
.mover {
  padding-left: 9em;
  font-size: 1em;
}

.full-width {
  width: 100%;
}

.centered-text {
  justify-content: space-between;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  font-family: 'Raleway', italic;
  font-size: 3dvh;
  padding-right: 5em;
  color: white;
  padding-bottom: 5em; /* Aumentar el margen inferior para un espacio mayor */
}

.playfair-display {
  font-family: 'Playfair Display', serif;
  font-style: italic;
  font-size: 15vh;
  line-height: 1em;
  color: rgb(255, 255, 255);
}

.playfair-display .coming {
  position: relative;
}

.playfair-display .soon {
  position: relative;
  margin-left: -2.52em;
  top: 0.55em;
}

.bottom-text {
  margin-top: 4em;
  padding-left: 9em;
  /* Ajusta el margen superior según tus preferencias */
}

/* Media query para pantallas con un ancho máximo de 800px (ajustado para dispositivos móviles) */
@media (max-width: 800px) {
  .mover {
    padding-left: 0;
  }
}
</style>
