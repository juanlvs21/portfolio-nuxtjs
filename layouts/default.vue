<template>
  <b-row class="w-100 m-0">
    <b-col cols="3" class="p-0">
      <Sidenav />
    </b-col>
    <b-col cols="9" class="p-0">
      <nuxt />
    </b-col>
  </b-row>
</template>

<script>
// Components
import Sidenav from '~/components/core/Sidenav'

export default {
  name: 'DefaultLayout',
  components: {
    Sidenav
  }
}
</script>