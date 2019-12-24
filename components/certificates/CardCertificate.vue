<template>
  <u-animate-container>
    <u-animate
      name="animated"
      delay="0s"
      duration="1s"
      :iteration="1"
      :offset="0"
      animateClass="zoomIn"
      :begin="false"
    >
      <b-card no-body class="overflow-hidden card-certificate mt-3">
        <b-row no-gutters>
          <b-col
            lg="6"
            md="12"
            sm="12"
            class="d-flex justify-content-center align-items-center card-col-img"
          >
            <b-card-img :src="`/badge/${certificate.img}`" class="rounded-0 card-badge"></b-card-img>
          </b-col>
          <b-col lg="6" md="12" sm="12" class="d-flex justify-content-center align-items-center">
            <b-card-body :title="certificate.name">
              <b-card-text>{{ certificate.date }}</b-card-text>
            </b-card-body>
          </b-col>
        </b-row>
      </b-card>
    </u-animate>
  </u-animate-container>
</template>

<script>
// Imports
import { UAnimateContainer, UAnimate } from 'vue-wow'

export default {
  name: 'CardCertificate',
  props: ['certificate'],
  components: {
    UAnimateContainer,
    UAnimate
  }
}
</script>

<style>
.card-certificate {
  height: 150px;
  transition: top ease 0.3s;
  top: 0px;
}

.card-certificate .card-title {
  font-size: 16px;
  font-weight: bold;
}

.card-certificate:hover {
  border: 1px solid #17a2b8;
  -webkit-box-shadow: 5px 5px 5px 0px rgba(0, 0, 0, 0.2);
  -moz-box-shadow: 5px 5px 5px 0px rgba(0, 0, 0, 0.2);
  box-shadow: 5px 5px 5px 0px rgba(0, 0, 0, 0.2);
  top: -5px;
}

.card-badge {
  width: 100px;
  height: 100px;
}

.card-col-img {
  height: 150px;
}

@media screen and (max-width: 991px) {
  .card-certificate {
    height: 250px;
  }
  .card-col-img {
    height: 120px;
  }
}

@keyframes moveHover {
  from {
    -webkit-transform: scale3d(0.3, 0.3, 0.3);
    transform: scale3d(0.3, 0.3, 0.3);
  }
}
</style>