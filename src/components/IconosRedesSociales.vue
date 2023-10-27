<template>
  <div class="mover">
    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a href="https://www.instagram.com" target="_blank">
            <svg-icon type="mdi" :path="instagram"></svg-icon>
          </a>
        </v-btn>
        <br>
        <br>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a href="https://www.linkedin.com" target="_blank">
            <svg-icon type="mdi" :path="linkedin"></svg-icon>
          </a>
        </v-btn>
        <br>
        <br>
      </v-col>
    </v-row>

    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a href="https://www.facebook.com" target="_blank">
            <svg-icon type="mdi" :path="facebook"></svg-icon>
          </a>
        </v-btn>
        <br>
        <br>
      </v-col>
    </v-row>

    <v-row>
      <v-col class="icon-col">
        <v-btn>
          <a :href="getWhatsAppLink()" target="_blank">
            <svg-icon type="mdi" :path="whatsapp"></svg-icon>

          </a>
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiInstagram } from '@mdi/js';
import { mdiWhatsapp } from '@mdi/js';
import { mdiFacebook } from '@mdi/js';
import { mdiLinkedin } from '@mdi/js';
</script>

<script>
export default {
  name: "my-component",
  components: {
    SvgIcon
  },
  data() {
    return {
      instagram: mdiInstagram,
      whatsapp: mdiWhatsapp,
      facebook: mdiFacebook,
      linkedin: mdiLinkedin,
    }
  },
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
.mover {
  margin-right: 8vh;
  color: white;
}
</style>