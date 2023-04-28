<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Merchandise from './components/Merchandise.vue';
import links from './components/links.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'app',
  components: {
    Header,
    Main,
    Merchandise,
    links,
    Footer,
  }

}
</script>

<template>
  <main id="main_wrapper" class="">

    <Header/>
    <Main/>
    <Merchandise/>
    <links/>
    <Footer/>

  </main>  
</template>

<style lang="scss">
@import './scss/main.scss';



</style>
