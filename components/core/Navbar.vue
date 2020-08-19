<template>
  <b-navbar toggleable="lg" type="dark" variant="info" sticky>
    <b-navbar-brand href="#">Juanlvs</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <li class="nav-item">
          <nuxt-link :to="{ path: '/' }" class="nav-link">Inicio</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/certificaciones' }" class="nav-link">Certificaciones</nuxt-link>
        </li>

        <!-- <li class="nav-item">
          <nuxt-link :to="{ path: '/portafolio' }" class="nav-link">Portafolio</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/blog' }" class="nav-link">Blog</nuxt-link>
        </li>

        <li class="nav-item">
          <nuxt-link :to="{ path: '/contacto' }" class="nav-link">Contacto</nuxt-link>
        </li> -->

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

.menu-dropdown li .dropdown-item:hover {
  background-color: #17a2b8 !important;
  color: #fff !important;
}

.menu-dropdown li .nuxt-link-exact-active {
  font-weight: bold;
  color: #17a2b8 !important;
}
</style>
