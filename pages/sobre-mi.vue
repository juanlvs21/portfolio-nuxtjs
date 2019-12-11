<template>
  <div>
    <ToolImg height="100vh" class="position-absolute" style="z-index: -100" />
    <section class="container pt-5 text-white about-container">
      <div class="text-center">
        <h1>¿Quién soy?</h1>
      </div>
      <div class="text-about mt-4">
        <p>Soy Juan Villarroel, venezolano estudiante de Licenciatura en Informática. Siempre he tenido como hábitat natural el entorno de la programación web, tanto a nivel informativo como laboral. En el transcurso de mi carrera universitaria siempre he buscado información adicional relacionada al diseño web, he realizado varios proyectos por hobbie. Adicionalmente poseo conocimientos prácticos en el uso de Photoshop siendo un gran apoyo en el diseño de algún proyecto. Me considero una persona con compromiso, y por poner mucho empeño en las cosas hago, programar para mi se vuelve entretenido, me divierte, me emociona. Es por eso que cuando se trata de programar siempre doy el 200% de mi y así enfrentar todas las dificultades al momento de proponerme algo.</p>
      </div>
    </section>
  </div>
</template>

<script>
// Components
import ToolImg from '~/components/core/ToolImg'

export default {
  name: 'SobreMiPage',
  components: {
    ToolImg
  }
}
</script>

<style>
.text-about {
  text-align: justify;
  line-height: 26px;
}
</style>