<template>
  <u-animate-container>
    <u-animate
      :name="animated"
      delay="0s"
      duration="1s"
      :iteration="1"
      :offset="0"
      animateClass="animated"
      :begin="false"
    >
      <b-card
        :img-src="imgPath"
        :img-alt="alt"
        :img-left="left"
        :img-right="right"
        class="mb-3 card-home"
        :class="[textPosition]"
      >
        <b-card-body>
          <h5>
            <b>{{ title }}</b>
          </h5>
          <p class="text-16px">
            {{ text }}
          </p>
        </b-card-body>
      </b-card>
    </u-animate>
  </u-animate-container>
</template>

<script>
// Imports
import { UAnimateContainer, UAnimate } from 'vue-wow'

export default {
  name: 'ReasonCard',
  props: ['title', 'text', 'img', 'alt', 'right', 'left'],
  components: {
    UAnimateContainer,
    UAnimate
  },
  data() {
    return {
      imgPath: `/icons/${this.img}`,
      animated: this.left ? 'fadeInLeft' : 'fadeInRight',
      textPosition: this.left ? 'text-left' : 'text-right'
    }
  }
}
</script>

<style>
.card-home img {
  width: 100px;
}
.card-home .card-img-left {
  margin-left: 30px;
}
.card-home .card-img-right {
  margin-right: 30px;
}
.card-home:hover {
  border: 1px solid #ff7e67;
  -webkit-box-shadow: 5px 5px 5px 0px rgba(0, 0, 0, 0.2);
  -moz-box-shadow: 5px 5px 5px 0px rgba(0, 0, 0, 0.2);
  box-shadow: 5px 5px 5px 0px rgba(0, 0, 0, 0.2);
}
</style>
