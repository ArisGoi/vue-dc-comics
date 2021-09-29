<template>
  <div id="app">

    <Header/>

    <main>
      <p style="color: white">--> Content Goes Here</p>
    </main>
    <dcIndexBar/>

    <Footer/>

  </div>
</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import dcIndexBar from './components/main/dcIndexBar.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    dcIndexBar
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
