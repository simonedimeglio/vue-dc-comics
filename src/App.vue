<template>
  <div id="app">
    <Header />
    <Main />
    <Midnav />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Midnav from './components/Midnav.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Midnav,
    Footer
  }
}
</script>

<style lang="scss">
  @import "./style/app.scss";
</style>
