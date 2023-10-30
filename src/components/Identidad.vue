<template>
  <div class="center-content">
    <img class="palabra" src="@/assets/palabras.gif" alt="Palabras">
  </div>
</template>

<style scoped>
.palabra {
  height: auto;
  width: 50%;
  padding-bottom: 5rem;
}

.center-content {
  font-family: 'Playfair Display', serif; /* Cambiado a 'serif' ya que 'Playfair Display' no tiene una variante italic */
  font-weight: bold;
  font-style: italic;
  display: flex;
  justify-content: center;
  align-items: center;
  line-height: 1em;
  color: rgb(255, 255, 255);
  height: 100vh;
}
</style>
