<template>

  <div>

    <v-card
      flat
      tile
      dark
      class="blue darken-4 grey--text"
    >

      <v-container>
        <v-row justify="left">
          <v-col
            class="text-center"
            cols="12"
            sm="6"
            md="4"
          >

            <v-card-text class="white--text pt-4">
              <h1
                class="text-center "
                id="Marcas"
              >ELECTRONICA VALLE S.A. </h1>
              <br />
              Desarrollamos software en la medida de la necesidad del cliente,
              ofreciendo a las pequeñas y medianas empresas soluciones informáticas
            </v-card-text>
          </v-col>

          <v-col
            class="text-center"
            cols="12"
            sm="6"
            md="4"
          >

            <v-card-text class="white--text pt-4">
              <h1 class="text-center ">CONTACTO </h1>
              <br />
              <v-icon color=white>mdi-deskphone</v-icon>
              381 255-0906
              <br />
              <br />
              <v-icon color=white>mdi-deskphone</v-icon>
              381 255-0908
              <br />
              <br />
              <v-icon color=white>mdi-deskphone</v-icon>
              381 230-8659
              <br />
              <br />
              <v-icon color=white>mdi-whatsapp</v-icon>
              381 6981-780
              <br />
              <br />
              <v-icon color=white>mdi-gmail</v-icon>
              correo@electronicavalle.com.ar
            </v-card-text>
          </v-col>
          <v-col
            class="text-center"
            cols="2"
            sm="2"
            md="2"
          >
            <br />

            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14241.942665618715!2d-65.21750386864731!3d-26.82450098064881!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94225c054171f5c3%3A0xfe72e29f08418aa9!2sELECTRONICA%20VALLE%20S.A.!5e0!3m2!1ses!2sar!4v1624044525788!5m2!1ses!2sar"
              width="400"
              height="300"
              style="border:0;"
              allowfullscreen=""
              loading="lazy"
            ></iframe>

          </v-col>
        </v-row>
        <v-container>

        </v-container>

        <v-container class="text-center">
          <v-card
            flat
            tile
            href="http://www.electronicavalle.com.ar"
            color="blue darken-4"
          >
            <span class="white--text text-caption">{{ new Date().getFullYear() }} — <strong>Creado por Electrónica Valle S.A.</strong></span>

          </v-card>
        </v-container>
      </v-container>

    </v-card>
  </div>
</template>



<script>
export default {
  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
    ],
  }),
}
</script>