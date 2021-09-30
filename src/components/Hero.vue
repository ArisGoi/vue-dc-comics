<template>
  <section id="hero"></section>
</template>

<script>
export default {
  name: 'Hero',
}
</script>

<!-- Style SCSS -->
<style scoped lang="scss">
@import '../assets/style/style.scss';

  #hero{
      height: $heroHeight;
      position: relative;
      background-image: $heroBackgroundImg;
      background-size: cover;
  }
</style>
