<template>
  <div class="w-100" :class="[textPosition]">
    <u-animate-container>
      <u-animate
        name="zoomIn"
        delay="0s"
        duration="1s"
        :iteration="1"
        :offset="0"
        animateClass="animated"
        :begin="false"
      >
        <h1 class="m-4">{{ title }}</h1>
      </u-animate>
    </u-animate-container>
  </div>
</template>

<script>
// Imports
import { UAnimateContainer, UAnimate } from 'vue-wow'

export default {
  name: 'TitleSection',
  props: ['title', 'left'],
  components: {
    UAnimateContainer,
    UAnimate
  },
  data() {
    return {
      textPosition: this.left ? 'text-left' : 'text-right'
    }
  }
}
</script>
