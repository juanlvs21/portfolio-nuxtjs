<template>
  <div class="mb-5">
    <section class="banner">
      <img
        src="~assets/img/programmer.webp"
        class="programmer"
        width="200"
        alt="banner-programmer"
      />
      <div class="container text-white text-container">
        <h1>Juan Villarroel</h1>
        <h4>Desarrollador Web</h4>
        <div class="icons mt-1">
          <img src="~assets/icons/vuejs.png" width="30px" alt="Vuejs" />
          <img src="~assets/icons/django.svg" width="30px" alt="Vuejs" />
          <img src="~assets/icons/flutter.svg" width="20px" alt="Vuejs" />
        </div>
      </div>
    </section>
    <section class="container text-center">
      <h1 class="my-5">¿Por qué tener una página web?</h1>
      <b-row>
        <b-col sm="12" md="4" class="animated zoomIn">
          <img src="~assets/icons/group.svg" width="100px" alt="Clientes" />
          <h5 class="mt-2">
            <b>Atrae más clientes.</b>
          </h5>
          <p class="text-16px">
            En estos tiempos que corren, en la era del mundo online, se produce
            el fenómeno de la propagación a través de medios como el correo
            electrónico, Facebook u otras redes sociales, así como a través de
            los clásicos foros.
          </p>
        </b-col>
        <b-col sm="12" md="4" class="animated zoomIn">
          <img src="~assets/icons/growth.svg" width="100px" alt="Ventas" />
          <h5 class="mt-2">
            <b>Incrementa las ventas.</b>
          </h5>
          <p class="text-16px">
            Gracias a que las tiendas virtuales están disponibles 24/7, las
            ventas nunca se detienen y tus clientes siempre podrán visitarte. La
            comunicación con los usuarios mejora y las experiencia de compra, en
            la mayoria de los casos, siempre es positiva.
          </p>
        </b-col>
        <b-col sm="12" md="4" class="animated zoomIn">
          <img
            src="~assets/icons/shopping-bag.svg"
            width="100px"
            alt="Alcance"
          />
          <h5 class="mt-2">
            <b>Permite llegar a más mercados.</b>
          </h5>
          <p class="text-16px">
            No importa lo nueva o antugua que sea tu idea de negocio, si decides
            crear una página web, esta podrá competir con cualquier otro mercado
            y llegar hasta los lugares más lejanos del planeta.
          </p>
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
  transition: 'slide-up',
  components: {
    ToolImg
  }
}
</script>

<style>
.banner {
  background-image: url('~assets/img/tools.webp');
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 50vh;
  display: -webkit-box;
  display: flex;
  -webkit-box-align: center;
  align-items: center;
}
.banner .programmer {
  position: absolute;
  right: 10%;
  top: 12%;
}
.banner .text-container {
  z-index: 10;
}
.banner .text-container h1 {
  font-weight: bold;
}
.banner .icons {
  position: static;
}
.banner .icons img {
  margin-right: 15px;
}
</style>
