<template>
  <div class="d-flex align-center text-center">
    <div class="centered-text">
      <div class="caja1">
        <p class="mover">Contacto</p>
        <br>
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
  margin-bottom: 10em;
  margin-right: 15em;
}

.mover {
  padding-left: 13em;
  font-size: 1em;
  font-family: 'Raleway', 'sherif';
  font-size: 1.5em;
}

.email-link {
  font-size: 5em;
  text-decoration: none;
  color: inherit;
  cursor: pointer;
  font-family: 'Playfair Display', serif;
  font-weight: bold;
  font-style: italic;
  margin-left: 4em;
}

.bottom-text {
  padding-left: 13em;
  font-size: 1em;
  font-family: 'Raleway', 'sherif';
  font-size: 1.5em;
}

.numero {
  font-family: 'Playfair Display', 'italic';
  font-style: italic;
  padding-left: 0.5em;
  font-size: 3em;
}

.horario {
  margin-top: 0.2em;
  padding-left: 1em;
}

.centered-text {
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  color: white;
}

.mobile-icons {
  display: none;
  flex-direction: row;
  justify-content: center;
}

/* Media query para pantallas con un ancho máximo de 800px (ajustado para dispositivos móviles) */
@media (max-width: 800px) {
  .mover {
    padding-left: 0;
    font-size: 3vh;
    /* Ajusta el tamaño de fuente para dispositivos móviles */
  }

  .bottom-text {
    font-size: 4vh;
    /* Ajusta el tamaño de fuente para dispositivos móviles */
  }

  .email-link {
    font-size: 4vh;
    /* Ajusta el tamaño de fuente para dispositivos móviles */
  }

  .mobile-icons {
    display: flex;
    flex-direction: column;
  }
}</style>
