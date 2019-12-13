<template>
  <b-navbar toggleable="lg" type="dark" sticky class="bg-gradient">
    <!-- <img src="https://placekitten.com/g/30/30" class="d-inline-block align-top" alt="Kitten" /> -->
    <b-navbar-brand href="#">Juancode</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <li class="nav-item">
          <nuxt-link :to="{ path: '/' }" class="nav-link">Inicio</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/sobre-mi' }" class="nav-link">Sobre mi</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/portafolio' }" class="nav-link">Portafolio</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/blog' }" class="nav-link">Blog</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/contacto' }" class="nav-link">Contacto</nuxt-link>
        </li>

        <!-- <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
        </b-nav-item-dropdown>-->

        <!-- <b-nav-item-dropdown right>
          <template v-slot:button-content>
            <em>User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>-->
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style >
.nuxt-link-exact-active {
  font-weight: bold;
  color: #fff !important;
}
.bg-gradient {
  background: #42b883; /* fallback for old browsers */
  background: -webkit-linear-gradient(
    to left,
    #42b883,
    #347474
  ); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(
    to left,
    #42b883,
    #347474
  ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
</style>