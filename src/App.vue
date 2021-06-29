<template>
  <v-app>
    <v-card class="overflow-hidden">
      <v-app-bar
        id="app-bar-ev"
        app
        dark
        flat
        fade-img-on-scroll
      >

        <v-app-bar-nav-icon
          class="hidden-md-and-up"
          @click="drawer = !drawer"
          dark
          color="blue accent-4"
          medium
          elevation="5"
        />
        <v-toolbar-title>
          <div>
            <router-link to="/">
              <v-img
                id="logo"
                src="@/assets/logo_web.svg"
                contain
                height="50"
                max-width="350"
                position="left"
                class="animate__animated animate__fadeInUp"
              />

            </router-link>
          </div>
        </v-toolbar-title>
        <v-spacer></v-spacer>

        <div id="menuev">
          <v-tabs
            align-with-title
            background-color="transparent"
            class="hidden-sm-and-down font-weight-bold"
            :ripple="false"
            active-class="text--primary"
            min-width="96"
          >
            <v-tab @click="$vuetify.goTo('#Nosotros') ; drawer = false">NOSOTROS</v-tab>
            <v-tab @click="$vuetify.goTo('#Servicios') ; drawer = false">SERVICIOS</v-tab>
            <v-tab @click="$vuetify.goTo('#Clientes') ; drawer = false">CLIENTES</v-tab>
            <v-tab @click="$vuetify.goTo('#Contacto') ; drawer = false">CONTACTO</v-tab>
          </v-tabs>
        </div>
        <v-btn
          rounded
          color="primary"
          dark
          href="http://evsa2/ccd_cliente/static/tienda/#/"
          target="_blank"
          class="hidden-sm-and-down"
        >
          TIENDA
          <v-icon
            right
            dark
          >
            mdi-cart-arrow-right
          </v-icon>
        </v-btn>
        <v-btn icon>
          <v-icon class="hidden-sm-and-down">mdi-magnify</v-icon>
        </v-btn>
        <v-btn
          icon
          target="_blank"
          class="hidden-sm-and-down"
          href="http://evsa2/gra/login/index/login?_next=/gra/default/index"
        >
          <v-icon>mdi-account-circle-outline</v-icon>
        </v-btn>
      </v-app-bar>
    </v-card>

    <v-main>
      <router-view></router-view>
    </v-main>
    <evFooter />
  </v-app>
</template>

<script>
import evFooter from '@/components/evFooter'
export default {
  name: 'App',
  components: {
    evFooter,

  },
  data: () => ({
    //
  }),
};
</script>
<style>
#app-bar-ev {
  background-image: -webkit-linear-gradient(
    0deg,
    #ffffff 15%,
    rgb(0, 67, 252) 100%
  ) !important;
}

#app-bar-ev a {
  font-size: 14px;
  text-transform: uppercase !important;
}

#app-bar-ev h3 {
  font-size: 18px;
  font-family: "Nunito";
  font-weight: 500;

  text-decoration: none !important;
  padding: 5px;
  color: #ffffff;
  text-align: center;
  text-transform: none !important;
}
#app-bar-ev h3 strong {
  font-style: italic;
  font-size: 16px;
}

#logo {
  width: 90%;
}

.v-tab:hover {
  background-color: rgba(0, 0, 255, 0.2) !important;
}
#menuev a {
  text-decoration: none !important;
  color: black !important;
  font-family: "Nunito";
}
</style>


