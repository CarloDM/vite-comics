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
    <prova/>
  </div>
</template>


<style scoped>
.main{
  width: 100%;
  min-height: 120px;
}

</style>