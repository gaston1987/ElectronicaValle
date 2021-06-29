<template>
  <div id="clientes">

    <v-container
      fluid
      class="my-8"
    >
      <v-sheet
        class="mx-auto"
        flat
        max-width="100%"
      >
        <v-sheet>
          <h1
            class="text-center "
            id="Marcas"
          >MARCAS </h1>

        </v-sheet>
        <div class="divider"></div>
        <v-slide-group
          multiple
          show-arrows
        >
          <v-slide-item
            v-for="n in 20"
            :key="n"
          >

            <v-row>

              <v-col>
                <v-card
                  flat
                  elevation="10"
                >
                  <a
                    target="_blank"
                    href=""
                  > <img
                      :src="`data:image/png;base64,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`"
                      alt="Hasar"
                      class="clienteImg"
                    > </a>
                </v-card>

              </v-col>

              <v-col>
                <v-card
                  flat
                  elevation="10"
                >
                  <a
                    target="_blank"
                    href=""
                  > <img
                      :src="`data:image/jpeg;base64,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`"
                      alt="Kretz"
                      class="clienteImg"
                    > </a>
                </v-card>

              </v-col>

              <v-col>
                <v-card
                  flat
                  elevation="10"
                >
                  <a
                    target="_blank"
                    href=""
                  > <img
                      :src="`https://www.exportadoresdecordoba.com/images_db/logos/220px/15567_logo.jpg`"
                      alt="Systel"
                      class="clienteImg"
                    > </a>
                </v-card>

              </v-col>

              <v-col>
                <v-card
                  flat
                  elevation="10"
                >
                  <a
                    target="_blank"
                    href=""
                  > <img
                      :src="`data:image/png;base64,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`"
                      alt="Ubiquiti"
                      class="clienteImg"
                    > </a>
                </v-card>

              </v-col>

            </v-row>

          </v-slide-item>

        </v-slide-group>
      </v-sheet>

    </v-container>
  </div>
</template>



<script>
export default {
  data: () => ({
    model: null,
  }),
}
</script>


<style lang="scss" scoped>
$color-1: #0e40c6;
section {
  background-color: rgb(236, 236, 236);
  padding-top: 2em;
  padding-bottom: 2em;

  @media (max-width: 400px) {
    padding-top: 1em;
    padding-bottom: 1em;
  }
}

h1 {
  font-weight: 700;
}
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.titulo {
  font-family: "Poppins", sans-serif;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-size: 2em;
  color: $color-1;
}

.clienteImg {
  margin: 0.8em 1.3em;
  transition: filter 0.5s ease-in-out;
  max-height: 100px;

  &:hover {
    filter: grayscale(1);
  }

  @media (max-width: 600px) {
    max-height: 50px;
    margin: 0.8em 1.3em;
  }
}

@media only screen and (max-width: 600px) {
  #clientes img {
    min-height: 80px;
  }
}
</style>