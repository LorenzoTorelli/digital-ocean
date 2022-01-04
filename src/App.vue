<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './components/Macro/Header.vue'
import Main from './components/Macro/Main.vue'
import Footer from './components/Macro/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">
@import url("./assets/Variabili/Global.scss");
</style>
