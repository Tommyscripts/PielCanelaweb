<template>
    <div class="center-content">
      <img class="palabra" src="@/assets/palabras.gif" alt="Palabras">
    </div>
  </template>
  
  <style scoped>
  .palabra{
    height: auto;
    width: 50%;
  }
  .center-content {
    display: flex;
    justify-content: center; /* Centra horizontalmente */
    align-items: center; /* Centra verticalmente */
    font-family: 'Playfair Display', serif;
    font-size: 10vh;
    line-height: 1em;
    color: rgb(255, 255, 255);
    height: 100vh; /* Esto asegura que ocupe toda la altura de la pantalla */
  }
  </style>
  
  