<template>
  <div>
    <Navbar />
    <div class="content">
      <nuxt />
    </div>
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

<style>
body {
  overflow-y: scroll;
}
</style>