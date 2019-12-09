<template>
  <div class="tool-img" :style="{height: height}"></div>
</template>

<script>
export default {
  name: 'ToolImg',
  props: ['height']
}
</script>

<style>
.tool-img {
  width: 100%;
  background-image: url('~assets/img/tools.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>