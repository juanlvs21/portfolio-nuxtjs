<template>
  <b-container class="mb-5">
    <section class="mt-5 text-center">
      <h1>Certificaciones</h1>
    </section>
    <section class="mt-4">
      <div class="text-center">
        <h2>Carreras</h2>
      </div>
      <b-row class="d-flex justify-content-center">
        <b-col md="4" sm="12" v-for="(career, i) of careers" :key="i">
          <CardCertificate :certificate="career" />
        </b-col>
      </b-row>
    </section>
    <section class="mt-4">
      <div class="text-center">
        <h2>Cursos</h2>
      </div>
      <b-row class="d-flex justify-content-center">
        <b-col md="4" sm="12" v-for="(course, i) of courses" :key="i">
          <CardCertificate :certificate="course" />
        </b-col>
      </b-row>
    </section>
  </b-container>
</template>

<script>
// Components
import CardCertificate from '~/components/certificates/CardCertificate'

export default {
  name: 'CertificatesPage',
  transition: 'slide-up',
  components: {
    CardCertificate
  },
  data() {
    return {
      careers: [
        {
          name: 'Carrera de Desarrollo de Apps con React Native',
          date: '21/12/2019',
          img: 'carrera-react-native.webp'
        }
      ],
      courses: [
        {
          name: 'Fundamentos de IBM Cloud',
          date: '20/11/2018',
          img: 'ibm-cloud.webp'
        },
        {
          name: 'Fundamentos de Javascript',
          date: '14/03/2019',
          img: 'fundamentos-js.webp'
        },
        {
          name: 'Introducción a la Creación de Empresas y Startups',
          date: '06/04/2019',
          img: 'empresas-startups.webp'
        },
        {
          name: 'Curso de PHP con Laravel',
          date: '23/05/2019',
          img: 'laravel.webp'
        },
        {
          name: 'Curso Profesional de Vue.js',
          date: '07/06/2019',
          img: 'profesional-vuejs.webp'
        },
        {
          name: 'Curso de Django',
          date: '15/06/2019',
          img: 'django.webp'
        },
        {
          name: 'Fundamentos de Ingeniería de Software',
          date: '19/06/2019',
          img: 'fundamentos-ingenieria-software.webp'
        },
        {
          name: 'Curso de React.js',
          date: '17/07/2019',
          img: 'react-js.webp'
        },
        {
          name: 'Curso de React Router',
          date: '23/08/2019',
          img: 'react-router.webp'
        },
        {
          name: 'Curso de Next.js',
          date: '25/08/2019',
          img: 'next-js.webp'
        },
        {
          name: 'Curso de Gatsby',
          date: '03/09/2019',
          img: 'gatsby.webp'
        },
        {
          name: 'Curso de React Native',
          date: '02/10/2019',
          img: 'react-native.webp'
        },
        {
          name: 'Curso de Dart',
          date: '07/10/2019',
          img: 'dart.webp'
        },
        {
          name: 'Curso de React Navigation',
          date: '08/10/2019',
          img: 'react-navigation.webp'
        },
        {
          name: 'Curso de Flutter',
          date: '13/10/2019',
          img: 'flutter.webp'
        },
        {
          name: 'Curso de Inglés Básico para Principiantes',
          date: '28/10/2019',
          img: 'ingles-basico.webp'
        },
        {
          name: 'Curso de Ruby',
          date: '11/11/2019',
          img: 'ruby.webp'
        },
        {
          name: 'Curso de Progressive Web Apps con React.js',
          date: '18/12/2019',
          img: 'pwa-react-js.webp'
        }
      ]
    }
  }
}
</script>