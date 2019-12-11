<template>
  <div>
    <!-- <ToolImg height="40vh" /> -->
    <section class="container text-center">
      <h3 class="mt-4">¿Por qué tener una página web?</h3>
      <b-row>
        <b-col sm="12" md="4">
          <img src="~assets/svg/group.svg" width="100px" alt="Clientes" />
          <h5 class="mt-2">
            <b>Atrae más clientes.</b>
          </h5>
          <p
            class="text-16px"
          >En estos tiempos que corren, en la era del mundo online, se produce el fenómeno de la propagación a través de medios como el correo electrónico, Facebook u otras redes sociales, así como a través de los clásicos foros.</p>
        </b-col>
        <b-col sm="12" md="4">
          <img src="~assets/svg/growth.svg" width="100px" alt="Ventas" />
          <h5 class="mt-2">
            <b>Incrementa las ventas.</b>
          </h5>
          <p
            class="text-16px"
          >Gracias a que las tiendas virtuales están disponibles 24/7, las ventas nunca se detienen y tus clientes siempre podrán visitarte. La comunicación con los usuarios mejora y las experiencia de compra, en la mayoria de los casos, siempre es positiva.</p>
        </b-col>
        <b-col sm="12" md="4">
          <img src="~assets/svg/shopping-bag.svg" width="100px" alt="Alcance" />
          <h5 class="mt-2">
            <b>Permite llegar a más mercados.</b>
          </h5>
          <p
            class="text-16px"
          >No importa lo nueva o antugua que sea tu idea de negocio, si decides crear una página web, esta podrá competir con cualquier otro mercado y llegar hasta los lugares más lejanos del planeta.</p>
        </b-col>
      </b-row>
    </section>
  </div>
</template>

<script>
// Components
import ToolImg from '~/components/core/ToolImg'

export default {
  name: 'IndexPage',
  components: {
    ToolImg
  }
}
</script>
