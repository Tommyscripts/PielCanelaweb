<template>
    <v-app>
        <v-main>
            <v-container class="d-flex align-center text-center">
                <v-row>
                    <v-col>
                        <div class="centered-text">
                            <p>Próximamente</p>
                            <v-divider></v-divider>
                            <p class="playfair-display"> Coming soon</p>
                            <v-divider></v-divider>
                            Pronto podréis explorar una experiencia completamente nueva y mejorada.
                            <v-divider></v-divider>
                            ¡Mantente atento para descubrir nuestras novedades!
                        </div>
                    </v-col>
                </v-row>
            </v-container>
        </v-main>
    </v-app>
</template>
<script>

</script>
<style>

.centered-text {
    text-align: center;
    /* Alineación horizontal en el centro */
    display: flex;
    flex-direction: column;
    /* Alineación vertical en el centro */
    justify-content: center;
    height: 100vh;
    /* Centra verticalmente en la pantalla */
    font-family: Raleway;
}
.playfair-display {
  font-family: 'Playfair Display', serif;
  font-size: 15vh;
}
</style>