<template>
  <div>
    <Header/>
    <Jumbotrone/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Jumbotrone from './components/Jumbotrone.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Jumbotrone,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style/utilities.scss';
@import './assets/style/mix.scss';

</style>
