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
    <div class="container">
      
      <section class="debug">
        <div class="col debug"></div>
        <div class="col debug"></div>
        <div class="col debug"></div>
      </section>
      <div class="logo_bg debug"></div>

    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

.links{
  display: flex;
  width: 100%;
  height: 200px;
  background-image: url(../assets/vue-dc-comics-1/img/footer-bg.jpg);
  background-size: contain;
}
.links .container {
  @include FlexCenter;
  height: 100%;
}
section{
  display: flex;
  height: 100%;
}
section, .logo_bg {
  width: 50%;
  height: 100%;
}

.col{
  width: calc(100% /5);
  height: 100%;
}



</style>