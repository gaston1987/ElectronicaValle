<template>
  <v-container
    fluid
    class="my-8"
    id="nosotros"
  >
    <v-spacer></v-spacer>
    <h2
      class="pt-4 text-center"
      id="Nosotros"
      color="blue"
    >NOSOTROS</h2>
    <v-card
      class="pt-5"
      flat
      elevation="24"
      shaped
    >

      <v-card-text style="margin-top:10px; text-align:center;font-size:20px">
        MÁS DE 60 AÑOS DE TRAYECTORIA
        "Nuestra experiencia nos permite ofrecer a la pequeña y mediana empresa soluciones informáticas en la modalidad "llave en mano", combinando el mejor hardware en el mercado, con nuestro software de gestión , y un servicio de mantenimiento"
      </v-card-text>
    </v-card>

    <br />

    <v-row
      justify="space-around"
      no-gutters
    >
      <v-col class="col-md-4 col-xs-12">
        <v-card
          class="pt-10"
          flat
          elevation="24"
        >

          <v-spacer></v-spacer>

          <v-img
            src="https://www.pngitem.com/pimgs/m/534-5348813_software-development-company-png-transparent-png.png"
            height="200px"
          ></v-img>

          <v-card-title>
            DESARROLLO DE SOFTWARE
          </v-card-title>

          <v-card-subtitle>

          </v-card-subtitle>

        </v-card>

      </v-col>
      <v-col class="col-md-4 col-xs-12">
        <v-card
          class="pt-10"
          flat
          elevation="24"
        >

          <v-spacer></v-spacer>

          <v-card
            class="mx-auto"
            max-width="344"
          >
            <v-img
              src="https://www.sfperusac.com/images/services/Service1.png"
              height="200px"
            ></v-img>

            <v-card-title>
              Mantenimiento
            </v-card-title>

          </v-card>
        </v-card>

      </v-col>
      <v-col class="col-md-4 col-xs-12">
        <v-card
          class="pt-10"
          flat
          elevation="24"
        >

          <v-spacer></v-spacer>

          <v-card
            class="mx-auto"
            max-width="344"
          >
            <v-img
              src="https://t-position.com/wp-content/uploads/2016/02/UX-Rank-e-commerce.png"
              height="200px"
            ></v-img>

            <v-card-title>
              Venta de Hardware
            </v-card-title>
          </v-card>

        </v-card>

      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    show: false,
  }),
}
</script>

<style>
.subt1 h3 {
  font-size: 18px !important;
  color: #ffffff !important;
  font-style: normal !important;
  line-height: 22px;
}

.subt1 h2 {
  font-weight: bold;
}
</style>
