<template>
  <div>
    <Navbar />
    <div class="content">
      <nuxt />
    </div>
    <!-- <Footer /> -->
  </div>
</template>

<script>
// Components
import Sidenav from '~/components/core/Sidenav'
import Navbar from '~/components/core/Navbar'
import Footer from '~/components/core/Footer'

export default {
  name: 'DefaultLayout',
  components: {
    Sidenav,
    Navbar,
    Footer
  }
}
</script>

<style>
body {
  overflow-y: scroll;
}
</style>