<template>
  <div>
    <Navbar />
    <nuxt />
  </div>
</template>

<script>
// Components
import Sidenav from '~/components/core/Sidenav'
import Navbar from '~/components/core/Navbar'

export default {
  name: 'DefaultLayout',
  components: {
    Sidenav,
    Navbar
  }
}
</script>