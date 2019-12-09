<template>
  <aside class="h-screen bg-primary-page text-center text-white">
    <img src="~assets/img/avatar.jpg" class="sidenav-avatar" alt="Juanv" />
    <div>
      <h4 class="font-weight-bold">Juan Villarroel</h4>
      <p>Desarrollador Web</p>
    </div>
    <b-nav vertical class="w-100 text-white">
      <nuxt-link
        :to="{ path: '/' }"
        class="sidenav-items"
        :class="[itemSelected == '/' ? 'active': '']"
      >Inicio</nuxt-link>

      <nuxt-link
        :to="{ path: '/quien-soy' }"
        class="sidenav-items"
        :class="[itemSelected == '/quien-soy' ? 'active': '']"
      >¿Quién soy?</nuxt-link>

      <nuxt-link
        :to="{ path: '/certificaciones' }"
        class="sidenav-items"
        :class="[itemSelected == '/certificaciones' ? 'active': '']"
      >Certificaciones</nuxt-link>

      <nuxt-link
        :to="{ path: '/portafolio' }"
        class="sidenav-items"
        :class="[itemSelected == '/portafolio' ? 'active': '']"
      >Portafolio</nuxt-link>

      <nuxt-link
        :to="{ path: '/blog' }"
        class="sidenav-items"
        :class="[itemSelected == '/blog' ? 'active': '']"
      >Blog</nuxt-link>

      <nuxt-link
        :to="{ path: '/Contacto' }"
        class="sidenav-items"
        :class="[itemSelected == '/Contacto' ? 'active': '']"
      >Contacto</nuxt-link>
    </b-nav>
  </aside>
</template>

<script>
export default {
  name: 'Sidenav',
  head() {
    return {
      title: 'Juancode'
    }
  },
  computed: {
    itemSelected() {
      return this.$route.path
    }
  }
}
</script>

<style>
.sidenav-avatar {
  background-position: center;
  background-size: cover;
  width: 120px;
  height: 120px;
  border-radius: 50%;
  margin: 20px;
}

a.sidenav-items {
  padding: 10px;
  color: #fff;
}
a.sidenav-items :hover {
  font-weight: bold !important;
  color: red !important;
  text-decoration: none !important;
}

.sidenav-items.active {
  background-color: #ffffff21;
  margin: 5px 10%;
  font-weight: 800;
  border-radius: 20px;
  height: 40px;
}
</style>