<template>
  <!-- CLIENTES -->
  <section style="background-color: #f7f7f7;">
    <v-layout
      column
      wrap
      align-center
    >
      <v-flex
        xs12
        class="my-3"
      >
        <div class="text-xs-center">
          <v-spacer></v-spacer>
          <h2
            id="Clientes"
            color="blue"
          >CONFIARON EN NOSOTROS</h2>
        </div>
      </v-flex>
    </v-layout>

    <v-layout
      class="px-4 pb-3"
      wrap
    >
      <div class="text-xs-center mb-5">
        <a
          target="_blank"
          href="http://www.centrocard.com.ar/"
        > <img
            src="@/assets/centrocard2.png"
            alt="Centro Card"
            class="clienteImg"
          > </a>
        <a
          target="_blank"
          href="https://es-la.facebook.com/vineriasanjuan/"
        > <img
            src="@/assets/vineria.svg"
            id="vineria"
            alt="Vinería San Juan S.R.L"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.estructurasymandatos.com/"
        > <img
            src="@/assets/EM.png"
            alt="Estructuras y Mandatos"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.samericanfoods.com/"
        > <img
            src="@/assets/saf.png"
            alt="South American Foods"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.expresosanjose.com.ar/"
        > <img
            src="@/assets/ExpresoSanJose.jpg"
            alt="Expreso San José S.A."
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.agroworldexport.com.ar/"
        > <img
            src="@/assets/agroworld.png"
            alt="Agro World Group S.R.L."
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="https://www.facebook.com/pages/Distribuidora-Glefyc/491014130942920"
        > <img
            src="@/assets/Glefyc.png"
            alt="Glefyc S.R.L."
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.tartagal.gov.ar/"
        > <img
            src="@/assets/MuniTartagal.png"
            alt="Municipalidad de Tartagal"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.tinuvielservicios.com.ar/"
        > <img
            src="@/assets/tinuviel.jpg"
            alt="Tinuviel S.A."
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="https://tumejorcuota.com.ar/"
        > <img
            src="@/assets/tuMejorCuota.jpg"
            alt="Tu mejor cuota"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="https://www.gomezpardo.com.ar/"
        > <img
            src="@/assets/GomezPardo2.jpg"
            alt="Gomez Pardo"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="https://es-la.facebook.com/CasaElGato"
        > <img
            src="@/assets/casaElGato.jpeg"
            alt="Casa El Gato"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://www.avalonmotocenter.com.ar/"
        > <img
            src="@/assets/avalon3.jpg"
            alt="Avalón Moto Center"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://premiersrl.evsa.com.ar/busnelli/sitio#/Main"
        > <img
            src="@/assets/scjohnson_logo_hr.jpg"
            alt="Premier Distribuciones SRL"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href="http://limplus.com.ar"
        > <img
            src="@/assets/limplus.png"
            alt="Limplus"
            class="clienteImg"
          ></a>

        <a
          target="_blank"
          href=""
        > <img
            src="@/assets/wolf.jpeg"
            alt="Wolfs"
            class="clienteImg"
          ></a>

        <a
          target="_blank"
          href=""
        > <img
            src="@/assets/gerala.png"
            alt="Gerala"
            class="clienteImg"
          ></a>
        <a
          target="_blank"
          href=""
        > <img
            src="@/assets/tauil.jpeg"
            alt="Tauil"
            class="clienteImg"
          ></a>

        <a
          target="_blank"
          href=""
        > <img
            src="@/assets/distriuruguay.png"
            alt="Distribuidora Uruguay"
            class="clienteImg"
          ></a>

        <a
          target="_blank"
          href=""
        > <img
            src="@/assets/argentia_web.png"
            alt="Argentia"
            class="clienteImg"
          ></a>

        <a
          target="_blank"
          href=""
        > <img
            src="@/assets/alem500.jpeg"
            alt="Alem500"
            class="clienteImg"
          ></a>

      </div>
    </v-layout>

  </section>

</template>

<script>
export default {};
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

h1,
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

#vineria {
  max-height: 70px;

  @media (max-width: 600px) {
    max-height: 40px;
  }
}

.titulo {
  font-family: "Poppins", sans-serif;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-size: 2em;
  color: $color-1;
}

.clienteImg {
  filter: grayscale(1);
  height: 100px;
  margin: 0.8em 1.3em;
  transition: filter 0.5s ease-in-out;

  &:hover {
    filter: grayscale(0);
  }

  @media (max-width: 600px) {
    max-height: 50px;
    margin: 0.8em 1.3em;
  }
}
</style>