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

<style >

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.debug{
  background-color: rgba(255, 0, 0, 0.26);
  border: 1px solid black;
}

#main_wrapper{
  width: 100%;
  min-height: 300px;
  /* background-color: black; */
}


</style>
