<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p class="mover" >Próximamente</p>

      <div class="playfair-display">
        <span class="coming" >Coming</span>
        <span class="soon" >Soon</span>
      </div>
      
     
      <div class="bottom-text" >
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
/* Establece el estilo cursiva para todas las fuentes */
body {
  font-style: italic;
}

.mover {
  padding-left: 3em;
  font-size: 1em;
  font-family: 'Raleway', italic;
  font-style: italic;
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
  font-family: 'Raleway', sans-serif; /* Cambiado a 'sans-serif' ya que 'Raleway' no tiene una variante italic */
  font-size: 3dvh;
  padding-right: 4em;
  color: white;
  padding-bottom: 5em;
}

.playfair-display {
  font-family: 'Playfair Display', serif; /* Cambiado a 'serif' ya que 'Playfair Display' no tiene una variante italic */
  font-weight: bold;
  font-size: 200px;
  line-height: 1em;
  color: rgb(255, 255, 255);
  letter-spacing: 0.02em; /* Ajusta el valor según tus preferencias */
}

.playfair-display .coming {
  position: relative;
}

.playfair-display .soon {
  position: relative;
  margin-left: -2.9em;
  top: 0.6em;
}

.bottom-text {
  margin-top: 4em;
  padding-left: 9em;
  font-family: 'Raleway', italic;
  font-style: italic;
}

/* Media query para pantallas con un ancho máximo de 800px (ajustado para dispositivos móviles) */
@media (max-width: 800px) {
  .mover {
    padding-left: 0;
  }
}
</style>
