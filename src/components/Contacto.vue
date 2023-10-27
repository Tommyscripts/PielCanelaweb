<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p>Contacto</p>
      <br>
      <a class="email-link" href="mailto:hola@pielcaneladesign.com">
        <div class="playfair-display">
          hola@pielcaneladesign.com
        </div>
      </a>
      <br>
      <div class="bottom-text">
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

.email-link {
  text-decoration: none;
  color: inherit;
  cursor: pointer;
}

.mobile-icons {
  display: none;
  flex-direction: row;
  justify-content: center;
  margin-top: 1rem;
}

@media (max-width: 900px) {
  .mobile-icons {
    display: flex;
    flex-direction: column;
  }
}
</style>
