<template>
  <b-container class="mb-5">
    <section class="mt-5 text-center">
      <h1>Nueva Publicación</h1>
    </section>
    <section class="mt-4">
      <textarea v-model="input"></textarea>
      <div v-html="compiledMarkdown"></div>
    </section>
  </b-container>
</template>

<script>
// Imports
import marked from 'marked'

export default {
  name: 'BlogNewPage',
  transition: 'slide-up',
  head() {
    return {
      title: 'Blog - Nueva publicación | Juancode'
    }
  },
  data() {
    return {
      input: '# hello'
    }
  },
  computed: {
    compiledMarkdown() {
      return marked(this.input)
    }
  }
}
</script>
