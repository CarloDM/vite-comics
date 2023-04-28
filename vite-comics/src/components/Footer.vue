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
  <footer class="debug">
    <div class="container">
      <div class=" sign debug">
        <div class="botton debug"></div>
      </div>
  
      <div class="follow debug"></div>
    </div>
  </footer>
  
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

footer{
  width: 100%;
  height: 80px;
}
footer .container{
  @include FlexCenter;
}

.sign{
  width: 120px;
  height: 100%;
}
.follow{
  min-width: 300px;
  height: 100%;
}

</style>