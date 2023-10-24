<template>
  <div class="mover">
    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a href="https://www.instagram.com" target="_blank"><v-icon> Prueba 1</v-icon></a>
        </v-btn>
        <br>
      </v-col>
    </v-row>

    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a href="https://www.linkedin.com" target="_blank"><v-icon> Prueba 2</v-icon></a>
        </v-btn>
        <br>
      </v-col>
    </v-row>

    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a href="https://www.facebook.com" target="_blank"><v-icon> Prueba 3</v-icon></a>
        </v-btn>
        <br>
      </v-col>
    </v-row>

    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a :href="getWhatsAppLink()" target="_blank"><v-icon> Prueba 4</v-icon></a>
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  methods: {
    getWhatsAppLink() {
      // Número de teléfono (debe incluir el código de país, sin espacios ni caracteres especiales)
      const phoneNumber = "+34912516439";  // Reemplaza con el número de teléfono al que deseas enviar el mensaje

      // Mensaje opcional
      const message = "¡Hola! Estoy interesado en tu servicio.";

      // Formatea el enlace de WhatsApp
      const formattedMessage = encodeURIComponent(message);
      return `https://wa.me/${phoneNumber}?text=${formattedMessage}`;
    },
  },
};
</script>

<style>
.mover{
  margin-right: 8vh;
}
</style>