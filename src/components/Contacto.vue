<template>
  <div class="d-flex align-center text-center full-width">
    <div class="centered-text">
      <p style="font-style: italic;">Contacto</p>
      <br>
      <a class="email-link" href="mailto:hola@pielcaneladesign.com">
        <div class="playfair-display" style="font-style: italic;">
          hola@pielcaneladesign.com
        </div>
      </a>
      <br>
      <div class="bottom-text" style="font-size: 9vh; padding-left: 9em; font-family: 'Raleway', italic; padding-right: 7em;">
        912516439
        <br>
      </div>
      <div class="bottom-text2" style="font-size: 3vh; padding-left: 9em; font-family: 'Raleway', italic; padding-right: 2em;">
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
.bottom-text {
  font-size: 9vh;
  padding-left: 9em;
  font-family: 'Raleway', italic;
  padding-right: 7em;
}

.bottom-text2 {
  font-size: 3vh;
  padding-left: 9em;
  font-family: 'Raleway', italic;
  padding-right: 2em;
}

.centered-text {
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
  font-family: 'Raleway', italic;
  font-size: 8vh;
}

.playfair-display {
  font-family: 'PlayfairDisplay-Bolditalic', italic;
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

@media (max-width: 800px) {
  .mobile-icons {
    display: flex;
    flex-direction: column;
  }
}
</style>
