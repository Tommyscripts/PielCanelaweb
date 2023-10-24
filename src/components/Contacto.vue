<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p>Contacto</p>
      <v-divider></v-divider>
      <a class="email-link" href="mailto:hola@pielcaneladesign.com">
        <div class="playfair-display">
          hola@pielcaneladesign.com
        </div>
      </a>
      <v-divider></v-divider>
      <div class="bottom-text">
        912516439
        <br>
        Lunes a viernes de 10am-8pm
      </div>
    </div>
  </div>
</template>

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
  font-size: 3vh;
}

.playfair-display {
  font-family: 'Playfair Display', serif;
  font-size: 10vh;
  line-height: 1em;
  color: rgb(255, 255, 255);
}

.playfair-display .coming {
  position: relative;
}

.playfair-display .soon {
  position: relative;
  margin-left: -2.4em;
  top: 0.56em;
}

.email-link {
  text-decoration: none; /* Quita la subraya del enlace */
  color: inherit; /* Usa el color de texto predeterminado */
  cursor: pointer;
}
</style>
