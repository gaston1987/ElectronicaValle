<template>
  <v-container id="Servicios">

    <h1 class="text-center">SERVICIOS</h1>
    <v-card>
      <v-tabs
        color="blue darken-4"
        right
      >
        <v-tab>DESARROLLO DE SISTEMAS</v-tab>
        <v-tab>SOPORTE TECNICO</v-tab>
        <v-tab>HARDWARE</v-tab>

        <v-tab-item>
          <v-container fluid>
            <v-row>
              <v-col
                cols="12"
                md="4"
              >
                <p></p>
                <v-img
                  :src="`http://www.soluciones-interactivas.com/images/site/soporte-tecnico-web-barcelona-eduweb.png`"
                  aspect-ratio="1"
                  max-height="200"
                  max-width="250"
                ></v-img>
              </v-col>
              <v-col
                cols="6"
                md="4"
              >
                <p>Nuestra experiencia nos permite ofrecer a la pequeña y mediana empresa soluciones informáticas en la modalidad "llave en mano", combinando el mejor hardware en el mercado, con nuestro software de gestión , y un servicio de mantenimiento</p>
              </v-col>
            </v-row>
          </v-container>
        </v-tab-item>
        <v-tab-item>
          <v-container fluid>
            <v-row>
              <v-col
                cols="12"
                md="4"
              >
                <v-img
                  :src="`http://lbg-web.com.ar/wp-content/uploads/soportetecnico-300x300.png`"
                  aspect-ratio="1"
                  max-height="178"
                  max-width="250"
                ></v-img>
              </v-col>
              <v-col
                cols="12"
                md="4"
              >
                <p>Brindamos mantemiento para nuestros programas y servicio técnico para el hardware.</p>
              </v-col>
            </v-row>
          </v-container>
        </v-tab-item>
        <v-tab-item>
          <v-container fluid>
            <v-row>
              <v-col
                cols="12"
                md="4"
              >
                <v-img
                  :src="`https://image.freepik.com/vector-gratis/soporte-tecnico-personal-servicio-al-cliente_82574-6002.jpg`"
                  aspect-ratio="1"
                  max-height="178"
                  max-width="250"
                ></v-img>
              </v-col>

              <v-col
                cols="12"
                md="4"
              >
                <p>Ofrecemos hardware para mercados verticales (registradoras, puntos de venta, escáner y otros).</p>
              </v-col>
            </v-row>
          </v-container>
        </v-tab-item>
      </v-tabs>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: 'imgMenu',


  data: () => ({
    ecosystem: [
      {
        text: 'vuetify-loader',
        src: 'https://github.com/vuetifyjs/vuetify-loader',
      },
      {
        text: 'github',
        href: 'https://github.com/vuetifyjs/vuetify',
      },
      {
        text: 'awesome-vuetify',
        href: 'https://github.com/vuetifyjs/awesome-vuetify',
      },
    ],
    importantLinks: [
      {
        text: 'Documentation',
        href: 'https://vuetifyjs.com',
      },
      {
        text: 'Chat',
        href: 'https://community.vuetifyjs.com',
      },
      {
        text: 'Made with Vuetify',
        href: 'https://madewithvuejs.com/vuetify',
      },
      {
        text: 'Twitter',
        href: 'https://twitter.com/vuetifyjs',
      },
      {
        text: 'Articles',
        href: 'https://medium.com/vuetify',
      },
    ],
    whatsNext: [
      {
        text: 'Explore components',
        href: 'https://vuetifyjs.com/components/api-explorer',
      },
      {
        text: 'Select a layout',
        href: 'https://vuetifyjs.com/getting-started/pre-made-layouts',
      },
      {
        text: 'Frequently Asked Questions',
        href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
      },
    ],
  }),
}
</script>
<style>
#texto {
  font-family: "Nunito" !important;
}
</style>