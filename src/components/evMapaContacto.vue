
  <template>
  <v-container class="grey lighten-5">
    <h1
      class="transparent--text pt-3"
      id="Contacto"
    >CONTACTO</h1>
    <br>
    <br>
    <v-row no-gutters>
      <v-col>

        <v-card-text class="black--text pt-4">

        </v-card-text>
        <v-container>
          <v-img
            :src="`data:image/png;base64,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`"
            height="200"
            max-width="350"
            contain
            class="pm-6 mx-auto"
          />
        </v-container>

      </v-col>
      <v-col cols="1">

      </v-col>
      <v-col>
        <v-toolbar
          color="blue darken-3"
          cards
          dark
          flat
        >
          <v-icon style="#007ebf;  font-size:40px;">mdi-at</v-icon>
          <v-card-title
            class="font-weight-black"
            style="min-width:300px"
          >
            Contáctenos

          </v-card-title>
          <v-spacer></v-spacer>

        </v-toolbar>

        <v-card
          class="pa-6"
          outlined
          tile
          flat
        >
          <v-form
            ref="form"
            v-model="valid"
            lazy-validation
          >

            <v-text-field
              v-model="form['name']"
              dense
              :rules="nameRules"
              label="Apellido y Nombre"
              clearable
              required
              class="pr-10 pl-10"
            ></v-text-field>

            <v-row>
              <v-col
                cols="12"
                sm="6"
              >
                <v-text-field
                  v-model="form['tel_area']"
                  label="Cod.Area"
                  type="number"
                  dense
                  prefix="+54 - 0"
                  clearable
                  required
                  class="pr-10 pl-10"
                ></v-text-field>
              </v-col>
              <v-col
                cols="12"
                sm="6"
              >
                <v-text-field
                  v-model="form['tel_nro']"
                  type="number"
                  dense
                  label="Nro.Celular"
                  prefix="15"
                  clearable
                  required
                  class="pr-10 pl-10"
                ></v-text-field>
              </v-col>
            </v-row>

            <v-text-field
              v-model="form['email']"
              dense
              :rules="emailRules"
              label="E-mail"
              clearable
              required
              class="pr-10 pl-10"
            ></v-text-field>

            <v-textarea
              v-model="form.desMotivo"
              color="teal"
              class="pr-10 pl-10"
            >
              <template v-slot:label>
                <div>
                  Describinos tu consulta <small>(opcional)</small>
                </div>
              </template>
            </v-textarea>
            <v-row
              align="center"
              justify="center"
              mb-5
              style="margin-bottom:20px"
            >
              <v-btn
                :disabled="!valid"
                :small="$vuetify.breakpoint.mobile"
                color="info"
                @click="submitForm"
                rounded
              >
                Consultar
              </v-btn>

              <v-btn
                color="info"
                :small="$vuetify.breakpoint.mobile"
                @click="reset"
                rounded
              >
                Cancelar
              </v-btn>
            </v-row>

          </v-form>
          <v-dialog
            v-model="dialog"
            hide-overlay
            persistent
            width="300"
          >
            <v-card
              color="primary"
              dark
            >
              <v-card-text>
                Enviando...
                <v-progress-linear
                  indeterminate
                  color="white"
                  class="mb-0"
                ></v-progress-linear>
              </v-card-text>
            </v-card>
          </v-dialog>

          <v-dialog
            v-model="conf"
            hide-overlay
            persistent
            width="300"
          >
            <v-card
              color="#007ebf"
              dark
            >
              <v-card-title>
                Mensaje enviado con exito!

              </v-card-title>
              <v-card-text>
                Muchas gracias por su consulta, en breve nos comunicaremos con usted.

              </v-card-text>
              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn
                  color="white"
                  text
                  @click="conf = false"
                >
                  Cerrar
                </v-btn>

              </v-card-actions>
            </v-card>
          </v-dialog>
        </v-card>

      </v-col>
    </v-row>
  </v-container>
</template>


<script>
export default {
  name: 'mapaContacto',
  data () {

    return {
      form: {
        name: '',
        tel_area: '',
        tel_nro: '',
        email: '',
        desMotivo: '',
      },
      dialog: false,
      conf: false,
      valid: true,
      emailRules: [
        v => !!v || 'E-mail es requerido',
        v => /.+@.+\..+/.test(v) || 'E-mail debe ser válido',
      ],
      nameRules: [
        v => !!v || 'Nombre es requerido',
        v => (v && v.length >= 10) || 'La longitud del nombre debe ser mayor a 10 caracteres',
      ],
    }
  },
  methods: {

    submitForm () {
      if (!this.$refs.form.validate()) {
        return
      }
      this.dialog = true

      this.sendEmail()

    },

    sendEmail () {
      this.$loadScript("https://smtpjs.com/v3/smtp.js")
        .then(() => {                                         //this Promise return nothing!!!
          window.Email && window.Email.send({
            Host: "smtp.gmail.com",
            Username: "gaston.evsa@gmail.com",
            Password: "g32488379",

            To: 'gaston.evsa@gmail.com',
            From: "gaston.evsa@gmail.com",
            Subject: "Solicitud de Contacto WEB EVSA:" + this.form.name,
            Body: `<html>
                   <table style="border: 1px solid black">
                   <tr>
                   <td><strong>Apellido y Nombre:</strong></td>
                   <td>"${this.form.name}"</td>
                   </tr>
                   <tr>
                   <td><strong>Telefono:</strong></td>
                   <td>"${this.form.tel_area}-${this.form.tel_nro}"</td>
                   </tr>
                   <tr>
                   <td><strong>Email:</strong></td>
                   <td>"${this.form.email}"</td>
                   </tr>
                   <tr>
                   <td><strong>Motivo:</strong></td>
                   <td>"${this.form.desMotivo}"</td>
                   </tr>
                   </table>
                   </html>
                   `
          }).then(() => {
            this.dialog = false
            this.conf = true
            this.reset()
          }
          );
        })
        .catch((e) => {
          alert(e)
          this.dialog = false
          // Failed to fetch script
        })
    },



    reset () {
      this.$refs.form.reset()
    },

    resetValidation () {
      this.$refs.form.resetValidation()
    },
  },
}


</script>
