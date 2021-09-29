<template>
  <div id="app">

    <Header/>

    <main>

    </main>

    <Footer/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';
@import '@/assets/style/style.scss';

#app {
  margin-top: $header-height;
}
</style>
