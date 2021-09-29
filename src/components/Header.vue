<template>
  <header>
    <h1>Header pagina</h1>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  @import '@/assets/style/style.scss';

  header{
    position: fixed;
    top: 0;
    left: 0;
    height: 5rem;
    width: 100%;
    background-color: pink;
    display: flex;
  }
</style>
