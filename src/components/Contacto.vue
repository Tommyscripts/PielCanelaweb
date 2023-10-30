<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p class="mover">Contacto</p>
      <div class="bottom-text">
        <a class="email-link" href="mailto:hola@pielcaneladesign.com">hola@pielcaneladesign.com</a>
        <br>
        912516439
        <br>
        Lunes a viernes de 10am-8pm
      </div>
      <div class="mobile-icons">
        <v-icon>mdi-facebook</v-icon>
        <v-icon>mdi-twitter</v-icon>
        <v-icon>mdi-instagram</v-icon>
      </div>
    </div>
  </div>
</template>

<style scoped>
body {
  font-style: italic;
}
.full-width {
  width: 100%;
}
.bottom-text {
  font-size: 6vh;
  padding-left: 1em;
  font-family: 'Raleway', sans-serif;
}
.centered-text {
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  font-family: 'Raleway', sans-serif;
  font-size: 5vh;
  color: white;
}

.email-link {
  text-decoration: none;
  color: inherit;
  cursor: pointer;
  font-family: 'Playfair Display', serif;
  font-weight: bold;
  font-style: italic;
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
    font-size: 3vh; /* Ajusta el tamaño de fuente para dispositivos móviles */
  }
  .bottom-text {
    font-size: 4vh; /* Ajusta el tamaño de fuente para dispositivos móviles */
  }
  .email-link {
    font-size: 4vh; /* Ajusta el tamaño de fuente para dispositivos móviles */
  }
  .mobile-icons {
    display: flex;
    flex-direction: column;
  }
}
</style>
