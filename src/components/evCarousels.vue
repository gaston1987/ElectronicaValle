<template>

  <v-carousel
    hide-delimiters
    show-arrows-on-hover
    cycle
    dark
    continuous
    interval="5000"
    progress
    progress-color="secondary"
    class="mb-2 elevation-2"
    :show-arrows="false"
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    >

      <section id="section1">

        <div class="header-overlay">

          <div class="header-titulo-contenedor">

            <h1 class="white--text header-titulo">
              TECNOLOGIA A LA MEDIDA DE SU EMPRESA
            </h1>
          </div>

          <h2 class="white--text text-xs-center header-subtitulo">
            Desarrollamos e implementamos soluciones de sistemas de software personalizado, que se integra perfectamente con el hardware que vendemos, y ofrecemos servicio técnico para ambos.
          </h2>

        </div>

      </section>

    </v-carousel-item>

  </v-carousel>
</template>

<script>
export default {
  data () {
    return {
      items: [

        {
          src: 'https://miro.medium.com/max/3840/1*Xv37PaIjTqZzoWQUk-4arw.jpeg',
        },
        {
          src: 'https://infonegocios.info/uploads/systel-balanzas-interna1-cba.jpg',
        },
        {
          src: 'http://ecija.com/wp-content/uploads/2016/06/software-development.jpg',
        },




      ],
    }
  },
}
</script>

<style lang="scss" scoped>
$color-1: #0e40c6;
$color-2: #380ec6;
$color-3: #940ec6;
$color-4: #c60e9c;
$color-5: #c60e40;
$color-6: #c6380e;

.logochico {
  height: 40px;
}

.sidebar {
  margin-top: 3.5em;
  display: flex;
  flex-direction: column;
}

.toolbar {
  background-color: white;
  height: 90px;
  font-family: "Poppins", sans-serif;
  color: blue;
  width: 100%;
  position: fixed;
  z-index: 9999;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  &-chico {
    position: fixed;
    z-index: 999;
    background: white;
    height: 50px;
  }

  &-botones {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
  }

  &-title {
    font-family: "Sawarabi Gothic", sans-serif;
    font-size: 2.5em;
    padding-left: 1em;
    letter-spacing: 2px;
    font-variant: small-caps;
  }
}

#section1 {
  width: 100%;
  margin-top: 50px;

  background-position: center;
  background-size: cover;
  background-attachment: fixed;
  height: 600px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;

  @media (max-width: 600px) {
    margin-top: 0;
    height: 400px;
  }
}

.header {
  &-overlay {
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background: rgba($color: #000000, $alpha: 0.9);
    height: 300px;
    font-family: "Nunito" !important;

    @media (max-width: 600px) {
      margin-top: 0;
      height: 400px;
    }
  }

  &-texto {
    margin: 0 auto;
    width: 80%;
  }

  &-titulo {
    font-family: "Montserrat";
    font-style: normal;
    font-weight: 400;
    text-align: center;
    letter-spacing: 1px;
    font-size: 4em;

    &-contenedor {
      width: 80%;
    }

    @media (max-width: 600px) {
      font-size: 2.3rem;
      font-weight: 900;
      width: 80%;
      margin: 0 auto;
    }
  }

  &-subtitulo {
    font-family: "Poppins", sans-serif;
    width: 80%;
    letter-spacing: 1px;
    font-weight: 400;
    margin-top: 1em;
    font-size: 1.4em;

    @media (max-width: 600px) {
      font-size: 1em;
    }
  }
}
</style>