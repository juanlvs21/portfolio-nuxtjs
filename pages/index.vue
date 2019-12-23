<template>
  <div class="mb-5">
    <section class="banner">
      <img src="~assets/img/programmer.webp" class="programmer" width="200" alt="banner-programmer" />
      <div class="container text-white text-container">
        <h1>Juan Villarroel</h1>
        <h4>Desarrollador Web</h4>
        <div class="icons mt-1">
          <img src="~assets/icons/vuejs.png" width="30px" alt="Vuejs" />
          <img src="~assets/icons/django.svg" width="30px" alt="Django" />
          <img src="~assets/icons/flutter.svg" width="20px" alt="Flutter" />
        </div>
      </div>
    </section>
    <section class="container">
      <b-row>
        <TitleSection title="¿Por qué tener una página web?" :left="true" />
        <b-col md="12">
          <ReasonCard
            title="Atrae más clientes."
            text="En estos tiempos que corren, en la era del mundo online, se produce el fenómeno de la propagación a través de medios como el correo electrónico, Facebook u otras redes sociales, así como a través de los clásicos foros."
            img="group.svg"
            alt="Clientes"
            :right="false"
            :left="true"
          />
        </b-col>
        <b-col md="12">
          <ReasonCard
            title="Incrementa las ventas"
            text="Gracias a que las tiendas virtuales están disponibles 24/7, las ventas nunca se detienen y tus clientes siempre podrán visitarte. La comunicación con los usuarios mejora y las experiencia de compra, en la mayoria de los casos, siempre es positiva."
            img="growth.svg"
            alt="Ventas"
            :right="false"
            :left="true"
          />
        </b-col>
        <b-col md="12">
          <ReasonCard
            title="Permite llegar a más mercados."
            text="No importa lo nueva o antugua que sea tu idea de negocio, si decides crear una página web, esta podrá competir con cualquier otro mercado y llegar hasta los lugares más lejanos del planeta."
            img="shopping-bag.svg"
            alt="Mas mercados"
            :right="false"
            :left="true"
          />
        </b-col>
      </b-row>

      <b-row>
        <TitleSection title="¿Por qué tener una aplicación web?" :left="false" />
        <b-col md="12">
          <ReasonCard
            title="Automatización de procesos."
            text="Al automatizar los procesos de ejecución, tienes un mayor del negocio además de la gestión y agilidad de respuesta en el punto de venta, siendo mucho más eficiente, fortaleciendo el nivel servicio y la forma en que los clientes te perciben."
            img="automation.svg"
            alt="Procesos"
            :right="true"
            :left="false"
          />
        </b-col>
        <b-col md="12">
          <ReasonCard
            title="Estadísticas y analíticas."
            text="Esto facilita la identificación de tendencias y comportamientos de los usuarios, así como tambien permite un estudio detallado del funcionamiento de los procesos. El objetivo final es que la analítica digital se considere como un canal potencial más con el que conseguir los mejores resultados."
            img="analytics.svg"
            alt="Estadisticas"
            :right="true"
            :left="false"
          />
        </b-col>
      </b-row>

      <b-row>
        <TitleSection title="¿Por qué tener una aplicación móvil?" :left="true" />
        <b-col md="12">
          <ReasonCard
            title="Alcance."
            text="En la actualidad, prácticamente todas las personas cuentan con dispositivos móviles personales con los cuales interactúan todo el día en sus tareas cotidianas. Aquí es donde nace una gran oportunidad para las empresas de estar aún más cerca de sus clientes y crear otro canal de venta."
            img="smartphone.svg"
            alt="Moviles"
            :right="false"
            :left="true"
          />
        </b-col>
      </b-row>
    </section>
  </div>
</template>

<script>
// Components
import ToolImg from '~/components/core/ToolImg'
import TitleSection from '~/components/home/TitleSection'
import ReasonCard from '~/components/home/ReasonCard'

export default {
  name: 'IndexPage',
  transition: 'slide-up',
  components: {
    ToolImg,
    TitleSection,
    ReasonCard
  }
}
</script>

<style>
.banner {
  background-image: url('~assets/img/bg.png');
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
