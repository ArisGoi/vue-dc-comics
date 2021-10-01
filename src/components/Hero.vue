<template>
  <section id="hero" :style="`background-image: url(${imglink}); height:${height}`"></section>
</template>

<script>
export default {
  name: 'Hero',
  props:['imglink', 'height']
}
</script>

<!-- Style SCSS -->
<style scoped lang="scss">
@import '../assets/style/style.scss';

  #hero{
      position: relative;
      background-size: cover;
  }
</style>
