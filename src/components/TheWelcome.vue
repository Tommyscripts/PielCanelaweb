<template>
  <div class="d-flex align-center text-center">
    <div class="centered-text">
      <div class="caja1">
        <p class="mover">Próximamente</p>
        <div class="playfair-display">
          <span class="coming">Coming</span>
          <span class="soon">Soon</span>
        </div>
        <div class="bottom-text">
          Pronto podréis explorar una experiencia completamente nueva y mejorada.
          <br>
          ¡Mantente atento para descubrir nuestras novedades!
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.caja1{
  padding-right: 2em;
}

.mover {
  padding-left: 3.9em;
  font-size: 1em;
  font-family: 'Raleway', 'sherif';
  font-size: 0.8em;
}
.playfair-display {
  font-family: 'Playfair Display', serif;
  font-weight: bold;
  font-style: italic;
  font-size: 200px;
  line-height: 1em;
  color: rgb(255, 255, 255);
  letter-spacing: 0.02em;
}

.playfair-display .coming {
  position: relative;
}

.playfair-display .soon {
  position: relative;
  margin-left: -2.82em;
  top: 0.6em;
}

.bottom-text {
  margin-top: 7em;
  padding-left: 5em;
  font-family: 'Raleway', 'sherif';
  font-size: 0.8em;
}
.centered-text {
  justify-content: space-between;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  font-family: 'Raleway', sans-serif;
  font-size: 3dvh;
  padding-right: 4em;
  color: white;
  padding-bottom: 5em;
}


/* Media query para pantallas con un ancho máximo de 800px (ajustado para dispositivos móviles) */
@media (max-width: 800px) {
  .mover {
    padding-left: 6em;
  }

  .centered-text {
    font-size: 2.5dvh;
    /* Ajusta el tamaño de fuente para dispositivos móviles */
    padding-right: 2em;
    /* Ajusta el margen derecho para dispositivos móviles */
    padding-bottom: 3em;
    /* Ajusta el margen inferior para dispositivos móviles */
  }

  .playfair-display {
    font-size: 150px;
    /* Ajusta el tamaño de fuente para dispositivos móviles */
    letter-spacing: 0;
    /* Elimina el espaciado entre letras para dispositivos móviles */
  }

  .playfair-display .coming {
    margin-left: 0;
    /* Restablece el margen izquierdo para dispositivos móviles */
    top: 1;
    /* Restablece la posición superior para dispositivos móviles */
    text-align: center;
    /* Centra el texto en dispositivos móviles */

  }

  ;

  .playfair-display .soon {
    margin-left: 1;
    /* Restablece el margen izquierdo para dispositivos móviles */
    top: 1;
    /* Restablece la posición superior para dispositivos móviles */
    text-align: center;
    /* Centra el texto en dispositivos móviles */
  }

  .bottom-text {
    margin-top: 6em;
    /* Ajusta el margen superior para dispositivos móviles */
    padding-left: 5em;
    /* Ajusta el margen izquierdo para dispositivos móviles */
  }
}</style>
