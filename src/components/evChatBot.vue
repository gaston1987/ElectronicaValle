<template>
  <div class="text-center">
    <v-menu
      v-model="menu"
      :close-on-content-click="false"
      :nudge-width="200"
      offset-x
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="blue darken-4"
          v-bind="attrs"
          v-on="on"
          id="botw"
          elevation="24"
          fab
        >

          <v-avatar size="100">
            <img
              width="70px"
              src="@/assets/avatar_bot.png"
            />
          </v-avatar>

        </v-btn>

      </template>

      <v-card>
        <v-list>
          <v-list-item>
            <v-list-item-avatar>
              <img
                width="70px"
                src="@/assets/avatar_bot.png"
              />
            </v-list-item-avatar>

            <v-list-item-content>
              <v-list-item-title>ELECTRONICA VALLE S.A.</v-list-item-title>
              <v-list-item-subtitle>en línea</v-list-item-subtitle>
            </v-list-item-content>

            <v-list-item-action>
              <v-btn
                :class="fav ? 'green--text' : ''"
                icon
              >
                <v-icon>mdi-face-agent</v-icon>
              </v-btn>
            </v-list-item-action>
          </v-list-item>
        </v-list>

        <v-divider></v-divider>

        <v-list>
          <v-container>
            <v-card
              elevation="3"
              outlined
              shaped
              width="auto"
              color="white"
            >
              <v-card-text>
                <p
                  class="font-weight-black"
                  style="max-width: 20rem;"
                > 👋 Hola! Soy Guillo tu asistente virtual.
                  Tengo un equipo en Electrónica Valle que me está enseñando para poder ayudarte cada vez mejor.
                  ¿Elige una opción para poder ayudarte?</p>
              </v-card-text>
            </v-card>
          </v-container>
          <v-divider></v-divider>

        </v-list>

        <v-dialog
          v-model="dialog4"
          width="800"
        >
          <template v-slot:activator="{ on, attrs }">
            <v-list-item
              link
              v-bind="attrs"
              v-on="on"
            >
              <v-list-item-action>
                <v-icon>mdi-information</v-icon>
              </v-list-item-action>
              <v-list-item-title>INFO-FISCAL</v-list-item-title>

            </v-list-item>
          </template>
          <v-card>

            <v-list-item>
              <v-list-item-avatar>
                <v-img src="@/assets/avatar_bot.png"></v-img>
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>ELECTRONICA VALLE S.A.</v-list-item-title>
                <v-list-item-subtitle>en línea</v-list-item-subtitle>
              </v-list-item-content>

              <v-list-item-action>
                <v-btn
                  :class="fav ? 'green--text' : ''"
                  icon
                >
                  <v-icon>mdi-face-agent</v-icon>
                </v-btn>
              </v-list-item-action>
            </v-list-item>
            <v-container fluid>
              <v-card
                elevation="3"
                outlined
                shaped
                color="white"
              >
                <v-card-text>
                  <p
                    class="font-weight-black"
                    style="max-width: 40rem;"
                  > 📒 Información Fiscal.</p>
                </v-card-text>
              </v-card>
              <div class="divider"></div>

              <v-row>
                <v-col
                  cols="2"
                  md="12"
                >
                  <v-img src="@/assets/bannerEVSA.jpg"></v-img>

                </v-col>

              </v-row>

            </v-container>
            <v-divider></v-divider>

            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn
                color="primary"
                text
                @click="dialog4 = false"
              >
                Cerrar
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-dialog>

        <v-dialog
          v-model="dialog2"
          width="500"
        >
          <template v-slot:activator="{ on, attrs }">
            <v-list-item
              link
              v-bind="attrs"
              v-on="on"
            >
              <v-list-item-action>
                <v-icon>mdi-clock-outline</v-icon>
              </v-list-item-action>
              <v-list-item-title>HORARIOS</v-list-item-title>
            </v-list-item>
          </template>
          <v-card>
            <v-list-item>
              <v-list-item-avatar>
                <v-img src="@/assets/avatar_bot.png"></v-img>
              </v-list-item-avatar>

              <v-list-item-content>
                <v-list-item-title>ELECTRONICA VALLE S.A</v-list-item-title>
                <v-list-item-subtitle>en línea</v-list-item-subtitle>
              </v-list-item-content>

              <v-list-item-action>
                <v-btn
                  :class="fav ? 'green--text' : ''"
                  icon
                >
                  <v-icon>mdi-face-agent</v-icon>
                </v-btn>
              </v-list-item-action>
            </v-list-item>
            <v-container>
              <v-card
                elevation="3"
                outlined
                width="auto"
                color="white"
              >
                <v-card-text>
                  <p
                    class="font-weight-black"
                    style="max-width: 40rem;"
                  > 🕘 Nuestros horarios de atención son los siguientes:</p>
                  <P>LUNES A VIERNES DE 8hs a 18hs</P>
                  <P>SÁBADOS DE 8:30hs a 12:30hs</P>
                </v-card-text>
              </v-card>
            </v-container>
            <v-divider></v-divider>

            <v-divider></v-divider>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn
                color="primary"
                text
                @click="dialog2 = false"
              >
                Cerrar
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-dialog>
        <v-list-item
          link
          href="https://api.whatsapp.com/send?phone=5493816981780"
          target="blank"
        >
          <v-list-item-action>

            <v-icon>mdi-whatsapp</v-icon>

          </v-list-item-action>
          <v-list-item-title>CHATEÁ CON NOSOTROS!</v-list-item-title>
        </v-list-item>
        <v-divider></v-divider>
      </v-card>

    </v-menu>
  </div>
</template>

<script>

export default {

  name: 'dialogChat',
  data () {
    return {

      fav: true,
      menu: false,
      message: false,
      hints: true,
      dialog: false,
      dialog2: false,
      dialog3: false,
      dialog4: false,
      dialog5: false,
    }
  },
  methods: {

    reset () {
      this.$refs.form.reset()
    },

    resetValidation () {
      this.$refs.form.resetValidation()
    },
  },
}
</script>
<style>
.b-agent-demo .b-agent-demo_powered_by {
  display: none !important;
}
#botw {
  position: fixed;
  bottom: 0;
  right: 0;
  z-index: 10;
}
#cns-cred {
  font-family: "Nunito" !important;
}
</style>
