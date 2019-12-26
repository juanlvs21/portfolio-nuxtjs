<template>
  <div>
    <div class="bg-title d-flex justify-content-md-center align-items-center">
      <h1 class="blog_title">{{ $route.params.post }}</h1>
      <Hola>
        <h1>Hola</h1>
      </Hola>
    </div>
  </div>
</template>

<script>
import Hola from '~/components/core/Hola'

export default {
  name: 'PostPage',
  transition: 'slide-up',
  head() {
    return {
      title: `${this.$route.params.post} | Juancode`
    }
  },
  components: {
    Hola
  }
}
</script>

<style>
.bg-title {
  background-image: url('~assets/img/bg-blog.webp');
  width: 100%;
}
.blog_title {
  margin: 60px 0px;
  color: #fff;
}
</style>
