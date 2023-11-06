<template>
  <div class="d-flex align-center text-center">
    <div class="centered-text">
      <div class="caja1">
        <p class="mover">CONTACTO</p>
        <a class="email-link" href="mailto:hola@pielcaneladesign.com">hola@pielcaneladesign.com</a>
        <div class="bottom-text">
          <div class="numero">
            912516439
          </div>
          <div class="horario">
            Lunes a viernes de 10am-8pm
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.caja1 {
  margin-left: 5em;
  margin-bottom: 10em;
  margin-top: 10em;
}

.mover {
  padding-right: 2em;
  font-family: 'Raleway', 'sherif';
  font-size: 0.5em;
  margin-top: 0; /* Agregado para ajustar el margen superior en dispositivos móviles */
}

.email-link {
  font-size: 4vh; /* Ajustado para dispositivos móviles */
  margin-left: 0; /* Eliminado el margen izquierdo en dispositivos móviles */
  padding-left: 0; /* Eliminado el margen izquierdo en dispositivos móviles */
  font-size: 3em;
  text-decoration: none; /* Corregido */
  cursor: pointer;
  font-family: 'Playfair Display', italic; /* Corregido */
  font-style: italic;
  color: white;
}

.bottom-text {
  font-size: 0.8em;
  padding-top: 0em;
}

.numero {
  font-size: 3.5em;
  font-family: 'Playfair Display', italic; /* Corregido */
  font-style: italic;
}

.horario {
  font-size: 0.8em;
  margin-top: 0.2em;
  padding-left: 1em;
}

.centered-text {
  justify-content: space-between;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  font-family: 'Raleway', sans-serif;
  font-size: 3vh;
  height: 100vh;
  padding-right: 4em;
  color: white;
  padding-bottom: 5em;
}

.mobile-icons {
  display: none; /* Asegúrate de controlar la visibilidad de los elementos en dispositivos móviles adecuadamente */
}

/* Media query para pantallas con un ancho máximo de 800px (ajustado para dispositivos móviles) */
@media (max-width: 800px) {
  .mover {
    padding-left: 6em;
  }

  .centered-text {
    font-size: 2.5vh;
    /* Ajusta el tamaño de fuente para dispositivos móviles */
    padding-right: 2em;
    /* Ajusta el margen derecho para dispositivos móviles */
    padding-bottom: 3em;
    /* Ajusta el margen inferior para dispositivos móviles */
  }

  .bottom-text {
    margin-top: 6em;
    /* Ajusta el margen superior para dispositivos móviles */
  }
}
</style>
