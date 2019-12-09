<template>
  <div>
    <ToolImg height="40vh" />
    <div class="container">
      <h1 class="title">juancode</h1>
      <h2 class="subtitle">My personal page, portfolio and blog</h2>
      <div class="links">
        <a href="https://nuxtjs.org/" target="_blank" class="button--green">Documentation</a>
        <a href="https://github.com/nuxt/nuxt.js" target="_blank" class="button--grey">GitHub</a>
      </div>
    </div>
  </div>
</template>

<script>
// Components
import ToolImg from '~/components/core/ToolImg'

export default {
  name: 'IndexPage',
  components: {
    ToolImg
  }
}
</script>
