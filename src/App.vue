<template>
  <div id="app">
    <Header />
    <Main :comics="comics" />
    <Midnav />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Midnav from './components/Midnav.vue';
import Footer from './components/Footer.vue';
import comicsJson from './jsons/dc-comics.json';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Midnav,
    Footer
  },
  data: function() {
    return {
      comics: comicsJson,
    };
  },
};
</script>

<style lang="scss">
  @import "./style/app.scss";
</style>
