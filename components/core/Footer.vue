<template>
  <div class="footer bg-gradient">
    <p class="text-center text-xs text-white m-2">
      &copy;{{ year }}
      <b>
        <a href="https://juancode.com.ve">Juancode</a> </b
      >. Todos los derechos reservados.
    </p>
  </div>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>

<style>
.footer {
  position: fixed;
  bottom: 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

.footer a {
  color: #ff7e67 !important;
}
</style>
