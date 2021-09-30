<template>
  <div id="app">

    <Header/>

    <Hero/>

    <main>
      <currentSeries/>
    </main>
    <dcIndexBar/>

    <Footer/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Hero from './components/Hero.vue'
import currentSeries from './components/main/currentSeries.vue'
import dcIndexBar from './components/main/dcIndexBar.vue'

export default {
  name: 'App',
  components: {
    currentSeries,
    Header,
    Footer,
    dcIndexBar,
    Hero
  }
}
</script>

<style lang="scss">
@import 'assets/style/variables.scss';
@import 'assets/style/style.scss';

#app {
  margin-top: $header-height;
}
</style>
