<script>
import prova from "../components/prova.vue";
export default {
  name: 'Header',
  components: {prova},
  data( ){
    return {
      
    }
  }
}
</script>

<template>
  <div class="main">
    <div class="container">

    <!-- <prova/> -->
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../scss/general.scss' as *;

.main{
  width: 100%;
  min-height: 120px;
}

.main .container {
  @include FlexCenter;
}

</style>