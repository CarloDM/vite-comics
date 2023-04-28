<script>
export default {
  name: 'Header',
  components: {},
  data( ){
    return {
      
    }
  }
}
</script>

<template>
  <div class="links debug">

    <section class="debug">
      <div class="col debug"></div>
      <div class="col debug"></div>
      <div class="col debug"></div>
    </section>
    <div class="logo_bg debug"></div>

  </div>
  
</template>


<style scoped>
.links{
  display: flex;
  width: 100%;
  height: 200px;
  background-image: url(../assets/vue-dc-comics-1/img/footer-bg.jpg);
  background-size: contain;
}
section{
  display: flex;
}
section, .logo_bg {
  width: 50%;
}

.col{
  width: calc(100% /5);
  height: 100%;
}



</style>