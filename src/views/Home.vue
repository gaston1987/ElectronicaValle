<template>
  <v-container fluid>
    <evCarousels />
    <div class="divider"></div>
    <div class="divider"></div>
    <evNosotros />
    <div class="divider"></div>
    <div class="divider"></div>
    <evParallax />
    <div class="divider"></div>
    <div class="divider"></div><br />
    <evServicios />
    <div class="divider"></div>
    <div class="divider"></div>
    <evMarcas />
    <div class="divider"></div>
    <div class="divider"></div>
    <evClientes />
    <div class="divider"></div>
    <div class="divider"></div>
    <evMapaContacto />
    <evChatBot />
  </v-container>
</template>

<script>
import evCarousels from '@/components/evCarousels'
import evNosotros from '@/components/evNosotros'
import evMarcas from '@/components/evMarcas'
import evParallax from '@/components/evParallax'
import evServicios from '@/components/evServicios'
import evClientes from '@/components/evClientes'
import evMapaContacto from '@/components/evMapaContacto'
import evChatBot from '@/components/evChatBot'

export default {
  name: 'Home',

  components: {
    evCarousels,
    evNosotros,
    evMarcas,
    evParallax,
    evServicios,
    evClientes,
    evMapaContacto,
    evChatBot,

  },
}
</script>
